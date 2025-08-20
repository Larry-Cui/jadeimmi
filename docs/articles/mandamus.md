---
title: 强制令简介及行业俗称解释
date: 2025-08-20
# authors:
tags:
  - Writ of Mandamus
  - Federal Court
draft: false
---

## 什么是强制令？

强制令（writ of *mandamus*）是一项司法救济，当移民申请遭受不合理的延误时，申请人可以请求联邦法院裁定，要求政府部门依法及时履行其审批职责，加快处理移民申请并做出决定。

强制令适用于各种移民申请，包括短期的旅游签、学签、工签，以及PR申请等。

强制令成功与否取决于两个关键因素：

- **不合理的延误：** 延误的时间长度将是一个重要因素，如果移民官的审理时间明显超出了通常的时限，这就可能被视为不合理。
- **政府是否有充分理由：** 如果移民官提供合理理由解释审批时间，则法院需要考虑此项因素。比方说，延误是因为移民官需要等待其它部门的安全审查结果，那合理的延期则应当视为正常情况。

## 强制令对申请人有没有负面影响？

没有。

## 强制令程序

强制令程序与普通诉讼基本一致。在该诉讼中，申请人作为原告，司法部（DOJ）的律师代表移民部作为被告。

- 提交申请（Serves/Files Application for Leave and for Judicial Review）。这是强制令的第一步。提交的表格是 Form IR-1。提交之后，申请人的电子邮箱会立刻受到法院的提交回执。然后两三个工作日后会受到法院要求付款的邮件，付款之后就算是提交成功。这一步的主要作用是让移民部知道，因为他们拖得太久了，你要对移民部采取法律手段了。这个阶段俗称“**强一**”。
- 完善申请人的起诉材料：这是正式整理证据并依法出诉求。通常这一步需要在提交申请后的30天内完成。在此过程中，很多情况下原被告双方可以进行协商、达成和解。如果移民部认可原告的请求合理，同意及时处理申请，原告可以撤诉。这个阶段俗称“**强二**”。
- 法院正式受理（Leave Decision）：如果法院受理，将会在大约90天内安排原被告双方开庭。这个阶段俗称“**强三**”。
- 开庭。
- 判决。

<h4 class="highlight red">现实中，很多强制令程序不会走到最后一步，而是会在上述诉讼程序的某一步结束。</h4>

## 强制令的可能结果

- 庭前撤诉：强一或强二阶段，双方达成和解，原告选择撤诉。
- 受理后撤诉：在法院受理后，双方在正式开庭前或判决前达成和解，原告选择撤诉。
- 驳回起诉：开庭审理后，法院驳回原告请求。
- 胜诉：开庭审理后，法院支持原告，裁定移民部在限时内做出行政决定。

## 从统计数据看强制令的效果

从2018年到2022年，在所有涉及移民局的40,767诉讼中，有1,358件是强制令申请。占比仅为3.3%。但从2018年以来，强制令申请数量几乎是逐年大幅度增加。

从2018年以来，强制令申请大多数以在庭前撤诉结束。庭前撤诉经常发生，是因为移民部收到强制令申请后会做一些相应的动作，比如发送补料信、要求进一步提供信息、甚至直接加速批准了强制令针对的申请事项。

<div id="piechart_div" style="width: 100%; height: 500px;"></div>

从2018年以来，强制令申请以在庭前撤诉结束的比例几乎是逐年上升。这意味着面对强制令，移民部越来越倾向于加快处理、促使强制令申请人撤诉。

<div id="myChart" style="max-width:100%; height:400px"></div>

## 参考资料

1. [Application for Leave and for Judicial review (Immigration) - TYPICAL STEPS IN AN APPLICATION FOR LEAVE AND FOR JUDICIAL REVIEW](https://www.fct-cf.gc.ca/en/pages/representing-yourself/procedural-charts/application-for-leave-and-for-judicial-review-immigration#cont){:target="\_blank"}
2. [Federal Courts Citizenship, Immigration and Refugee Protection Rules](https://laws.justice.gc.ca/eng/regulations/SOR-93-22/page-1.html#docCont){:target="\_blank"}
3. [Writ of Mandamus](https://www.holthelaw.com/writ-of-mandamus#:~:text=was%20not%20successful){:target="\_blank"}
4. [*Mandamus* Over the Years – A Stats Analysis: 2022 Spike + Increasing Discontinuance Rates](https://heronlaw.ca/mandamus-over-the-years-a-stats-analysis-2022-spike-increasing-discontinuance-rates/){:target="\_blank"}



<script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
<script type="text/javascript">

  google.charts.load('current', {'packages':['corechart']});
  google.charts.setOnLoadCallback(drawChart);

  function drawChart() {

// pie chart

    const data1 = google.visualization.arrayToDataTable([
      ['result', 'percentage'],
      ['庭前撤诉', 70.6],
      ['庭前驳回', 17.4],
      ['胜诉', 11.6],
      ['其它', 0.4],
    ]);

    const options1 = {
      title: '申请强制令的各种结果所占百分比(2018-2023)',
      pieHole: 0.4, // For a donut chart effect
    };

    const chart1 = new google.visualization.PieChart(document.getElementById('piechart_div'));
    chart1.draw(data1, options1);


// line chart

// Set Data
const data2 = google.visualization.arrayToDataTable([
  ['Price', 'Size'],
  ['2018',40],['2019',57],['2020',60],['2021',70],['2022',80],['2023',69]
  ]);
// Set Options
const options2 = {
  title: '庭前撤诉案件占比的年度趋势（%）',
  hAxis: {title: '年份'},
  vAxis: {title: '占所有强制令案件比例', minValue: 0, maxValue: 100},
  <!-- curveType: 'function', -->
  legend: 'none'
};
// Draw Chart
const chart2 = new google.visualization.LineChart(document.getElementById('myChart'));
chart2.draw(data2, options2);

  }




</script>