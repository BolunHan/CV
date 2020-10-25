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

Personal CV hosted by Github Pages

<ul>
    <li><a href="https://BolunHan.github.io/CV/en">CV-en</a></li>
    <li><a href="https://BolunHan.github.io/CV/zh">CV-zh</a></li>
</ul>

<ul>
    <li><a href="https://BolunHan.github.io/CV/en">英文简历</a></li>
    <li><a href="https://BolunHan.github.io/CV/zh">中文简历</a></li>
    <li><button id="cmd">Export PDF</button></li>
</ul>

last update: `2020-10-24`
