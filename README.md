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
    doc.save('cv.pdf');
});
</script>

# Personal CV of Han Bolun

<p>
Graduated from Peking University in 2016, majored in finance and physics, Han Bolun had joined CICC EQ. Department and became a cross-boarder sales trader. 

In 2017, I left CICC and joined the GLOBAL FORTUNE UNITED and started the career as an AI engineer focusing on short-term quantitative factor mining and Intraday trading.

In November 2022, I returned to campus to pursue an Master of Science in Applied Economics at Nanyang Technological University.
</p>

<p>
韩博伦毕业于北京大学元培学院，光华金融方向，2016年加入中金公司EQ部门成为一名跨境销售交易员。

2017年离开中金公司，加入上海鑫晟投资管理有限公司开始了量化工程师的职业生涯，专注于短线量化因子挖掘和日内交易。

2022年11月，我重返校园，在南洋理工大学攻读应用经济学硕士学位。
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
