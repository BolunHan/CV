<script>
var doc = new jsPDF();
var specialElementHandlers = {
    '#editor': function (element, renderer) {
        return true;
    }
};

$('#cmd').click(function () {
    doc.fromHTML($('#content').html(), 15, 15, {
        'width': 170,
            'elementHandlers': specialElementHandlers
    });
    doc.save('sample-file.pdf');
});
</script>

# Personal CV hosted by Github Pages

<p>
Graduated from Peking University in 2016, majored in finance and physics, Bolun Han had joined CICC EQ. Department and became a cross-boarder sales trader. In 2017, I left CICC and joined the GLOBAL FORTUNE UNITED and started the career as an AI engineer focusing on short-term quantitative factor mining and Intraday trading.
</p>

<ul>
    <li><a href="https://BolunHan.github.io/CV/en">CV-en</a></li>
    <li><a href="https://BolunHan.github.io/CV/zh">CV-zh</a></li>
</ul>

<ul>
    <li><a href="https://BolunHan.github.io/CV/en">英文简历</a></li>
    <li><a href="https://BolunHan.github.io/CV/zh">中文简历</a></li>
    <li><button id="cmd">Export PDF</button></li>
</ul>

last update: `2020-12-16`
