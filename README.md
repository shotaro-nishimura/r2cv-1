# r2cv-1: ROS2 Computer Vision お勉強ロボット(その1)
<html>
<head>
<meta http-equiv=Content-Type content="text/html; charset=shift_jis">
<meta name=Generator content="Microsoft Word 15 (filtered)">
<style>
<!--
 /* Font Definitions */
 @font-face
	{font-family:Wingdings;
	panose-1:5 0 0 0 0 0 0 0 0 0;}
@font-face
	{font-family:"Cambria Math";
	panose-1:2 4 5 3 5 4 6 3 2 4;}
@font-face
	{font-family:Calibri;
	panose-1:2 15 5 2 2 2 4 3 2 4;}
@font-face
	{font-family:"Wingdings 3";
	panose-1:5 4 1 2 1 8 7 7 7 7;}
@font-face
	{font-family:"Meiryo UI";
	panose-1:2 11 6 4 3 5 4 4 2 4;}
@font-face
	{font-family:メイリオ;
	panose-1:2 11 6 4 3 5 4 4 2 4;}
@font-face
	{font-family:"Segoe UI";
	panose-1:2 11 5 2 4 2 4 2 2 3;}
@font-face
	{font-family:Tahoma;
	panose-1:2 11 6 4 3 5 4 4 2 4;}
@font-face
	{font-family:"\@Meiryo UI";}
@font-face
	{font-family:"\@メイリオ";}
 /* Style Definitions */
 p.MsoNormal, li.MsoNormal, div.MsoNormal
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
h1
	{mso-style-link:"見出し 1 \(文字\)";
	margin-top:16.0pt;
	margin-right:0mm;
	margin-bottom:2.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:14.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	text-transform:uppercase;
	letter-spacing:.2pt;
	font-weight:bold;}
h2
	{mso-style-link:"見出し 2 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:14.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
h3
	{mso-style-link:"見出し 3 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	letter-spacing:.2pt;
	font-weight:normal;}
h4
	{mso-style-link:"見出し 4 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:normal;
	font-style:italic;}
h5
	{mso-style-link:"見出し 5 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
h6
	{mso-style-link:"見出し 6 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;
	font-style:italic;}
p.MsoHeading7, li.MsoHeading7, div.MsoHeading7
	{mso-style-link:"見出し 7 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-style:italic;}
p.MsoHeading8, li.MsoHeading8, div.MsoHeading8
	{mso-style-link:"見出し 8 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
p.MsoHeading9, li.MsoHeading9, div.MsoHeading9
	{mso-style-link:"見出し 9 \(文字\)";
	margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-style:italic;}
p.MsoIndex1, li.MsoIndex1, div.MsoIndex1
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:11.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex2, li.MsoIndex2, div.MsoIndex2
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:22.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex3, li.MsoIndex3, div.MsoIndex3
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:33.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex4, li.MsoIndex4, div.MsoIndex4
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:44.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex5, li.MsoIndex5, div.MsoIndex5
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:55.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex6, li.MsoIndex6, div.MsoIndex6
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:66.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex7, li.MsoIndex7, div.MsoIndex7
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:77.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex8, li.MsoIndex8, div.MsoIndex8
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:88.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndex9, li.MsoIndex9, div.MsoIndex9
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:99.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc1, li.MsoToc1, div.MsoToc1
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc2, li.MsoToc2, div.MsoToc2
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:11.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc3, li.MsoToc3, div.MsoToc3
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:22.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc4, li.MsoToc4, div.MsoToc4
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:33.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc5, li.MsoToc5, div.MsoToc5
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:44.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc6, li.MsoToc6, div.MsoToc6
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:55.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc7, li.MsoToc7, div.MsoToc7
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:66.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc8, li.MsoToc8, div.MsoToc8
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:77.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToc9, li.MsoToc9, div.MsoToc9
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:5.0pt;
	margin-left:88.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoNormalIndent, li.MsoNormalIndent, div.MsoNormalIndent
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoFootnoteText, li.MsoFootnoteText, div.MsoFootnoteText
	{mso-style-link:"脚注文字列 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoCommentText, li.MsoCommentText, div.MsoCommentText
	{mso-style-link:"コメント文字列 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoHeader, li.MsoHeader, div.MsoHeader
	{mso-style-link:"ヘッダー \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
p.MsoFooter, li.MsoFooter, div.MsoFooter
	{mso-style-link:"フッター \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoIndexHeading, li.MsoIndexHeading, div.MsoIndexHeading
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
p.MsoCaption, li.MsoCaption, div.MsoCaption
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:9.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
p.MsoTof, li.MsoTof, div.MsoTof
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoEnvelopeAddress, li.MsoEnvelopeAddress, div.MsoEnvelopeAddress
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:144.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoEnvelopeReturn, li.MsoEnvelopeReturn, div.MsoEnvelopeReturn
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
span.MsoFootnoteReference
	{font-family:"Meiryo UI";
	vertical-align:super;}
span.MsoCommentReference
	{font-family:"Meiryo UI";}
span.MsoLineNumber
	{font-family:"Meiryo UI";}
span.MsoPageNumber
	{font-family:"Meiryo UI";}
span.MsoEndnoteReference
	{font-family:"Meiryo UI";
	vertical-align:super;}
p.MsoEndnoteText, li.MsoEndnoteText, div.MsoEndnoteText
	{mso-style-link:"文末脚注文字列 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoToa, li.MsoToa, div.MsoToa
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:11.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-11.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoMacroText, li.MsoMacroText, div.MsoMacroText
	{mso-style-link:"マクロ文字列 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Meiryo UI";
	color:windowtext;}
p.MsoToaHeading, li.MsoToaHeading, div.MsoToaHeading
	{margin-top:6.0pt;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
p.MsoList, li.MsoList, div.MsoList
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListCxSpFirst, li.MsoListCxSpFirst, div.MsoListCxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListCxSpMiddle, li.MsoListCxSpMiddle, div.MsoListCxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListCxSpLast, li.MsoListCxSpLast, div.MsoListCxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet, li.MsoListBullet, div.MsoListBullet
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber, li.MsoListNumber, div.MsoListNumber
	{mso-style-link:"段落番号 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:39.6pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
p.MsoList2, li.MsoList2, div.MsoList2
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList2CxSpFirst, li.MsoList2CxSpFirst, div.MsoList2CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList2CxSpMiddle, li.MsoList2CxSpMiddle, div.MsoList2CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList2CxSpLast, li.MsoList2CxSpLast, div.MsoList2CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList3, li.MsoList3, div.MsoList3
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList3CxSpFirst, li.MsoList3CxSpFirst, div.MsoList3CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList3CxSpMiddle, li.MsoList3CxSpMiddle, div.MsoList3CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList3CxSpLast, li.MsoList3CxSpLast, div.MsoList3CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList4, li.MsoList4, div.MsoList4
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList4CxSpFirst, li.MsoList4CxSpFirst, div.MsoList4CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList4CxSpMiddle, li.MsoList4CxSpMiddle, div.MsoList4CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList4CxSpLast, li.MsoList4CxSpLast, div.MsoList4CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList5, li.MsoList5, div.MsoList5
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList5CxSpFirst, li.MsoList5CxSpFirst, div.MsoList5CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList5CxSpMiddle, li.MsoList5CxSpMiddle, div.MsoList5CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoList5CxSpLast, li.MsoList5CxSpLast, div.MsoList5CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet2, li.MsoListBullet2, div.MsoListBullet2
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet2CxSpFirst, li.MsoListBullet2CxSpFirst, div.MsoListBullet2CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet2CxSpMiddle, li.MsoListBullet2CxSpMiddle, div.MsoListBullet2CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet2CxSpLast, li.MsoListBullet2CxSpLast, div.MsoListBullet2CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet3, li.MsoListBullet3, div.MsoListBullet3
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet3CxSpFirst, li.MsoListBullet3CxSpFirst, div.MsoListBullet3CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet3CxSpMiddle, li.MsoListBullet3CxSpMiddle, div.MsoListBullet3CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet3CxSpLast, li.MsoListBullet3CxSpLast, div.MsoListBullet3CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet4, li.MsoListBullet4, div.MsoListBullet4
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet4CxSpFirst, li.MsoListBullet4CxSpFirst, div.MsoListBullet4CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet4CxSpMiddle, li.MsoListBullet4CxSpMiddle, div.MsoListBullet4CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet4CxSpLast, li.MsoListBullet4CxSpLast, div.MsoListBullet4CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet5, li.MsoListBullet5, div.MsoListBullet5
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet5CxSpFirst, li.MsoListBullet5CxSpFirst, div.MsoListBullet5CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet5CxSpMiddle, li.MsoListBullet5CxSpMiddle, div.MsoListBullet5CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListBullet5CxSpLast, li.MsoListBullet5CxSpLast, div.MsoListBullet5CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber2, li.MsoListNumber2, div.MsoListNumber2
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber2CxSpFirst, li.MsoListNumber2CxSpFirst, div.MsoListNumber2CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber2CxSpMiddle, li.MsoListNumber2CxSpMiddle, div.MsoListNumber2CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber2CxSpLast, li.MsoListNumber2CxSpLast, div.MsoListNumber2CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber3, li.MsoListNumber3, div.MsoListNumber3
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber3CxSpFirst, li.MsoListNumber3CxSpFirst, div.MsoListNumber3CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber3CxSpMiddle, li.MsoListNumber3CxSpMiddle, div.MsoListNumber3CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber3CxSpLast, li.MsoListNumber3CxSpLast, div.MsoListNumber3CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber4, li.MsoListNumber4, div.MsoListNumber4
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber4CxSpFirst, li.MsoListNumber4CxSpFirst, div.MsoListNumber4CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber4CxSpMiddle, li.MsoListNumber4CxSpMiddle, div.MsoListNumber4CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber4CxSpLast, li.MsoListNumber4CxSpLast, div.MsoListNumber4CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber5, li.MsoListNumber5, div.MsoListNumber5
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber5CxSpFirst, li.MsoListNumber5CxSpFirst, div.MsoListNumber5CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber5CxSpMiddle, li.MsoListNumber5CxSpMiddle, div.MsoListNumber5CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListNumber5CxSpLast, li.MsoListNumber5CxSpLast, div.MsoListNumber5CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoTitle, li.MsoTitle, div.MsoTitle
	{mso-style-link:"表題 \(文字\)";
	margin:0mm;
	text-align:center;
	font-size:24.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	letter-spacing:-.35pt;
	font-weight:bold;}
p.MsoTitleCxSpFirst, li.MsoTitleCxSpFirst, div.MsoTitleCxSpFirst
	{mso-style-link:"表題 \(文字\)";
	margin:0mm;
	text-align:center;
	font-size:24.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	letter-spacing:-.35pt;
	font-weight:bold;}
p.MsoTitleCxSpMiddle, li.MsoTitleCxSpMiddle, div.MsoTitleCxSpMiddle
	{mso-style-link:"表題 \(文字\)";
	margin:0mm;
	text-align:center;
	font-size:24.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	letter-spacing:-.35pt;
	font-weight:bold;}
p.MsoTitleCxSpLast, li.MsoTitleCxSpLast, div.MsoTitleCxSpLast
	{mso-style-link:"表題 \(文字\)";
	margin:0mm;
	text-align:center;
	font-size:24.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	letter-spacing:-.35pt;
	font-weight:bold;}
p.MsoClosing, li.MsoClosing, div.MsoClosing
	{mso-style-link:"結語 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:216.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoSignature, li.MsoSignature, div.MsoSignature
	{mso-style-link:"署名 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:216.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyText, li.MsoBodyText, div.MsoBodyText
	{mso-style-link:"本文 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyTextIndent, li.MsoBodyTextIndent, div.MsoBodyTextIndent
	{mso-style-link:"本文インデント \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue, li.MsoListContinue, div.MsoListContinue
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinueCxSpFirst, li.MsoListContinueCxSpFirst, div.MsoListContinueCxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinueCxSpMiddle, li.MsoListContinueCxSpMiddle, div.MsoListContinueCxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinueCxSpLast, li.MsoListContinueCxSpLast, div.MsoListContinueCxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue2, li.MsoListContinue2, div.MsoListContinue2
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue2CxSpFirst, li.MsoListContinue2CxSpFirst, div.MsoListContinue2CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue2CxSpMiddle, li.MsoListContinue2CxSpMiddle, div.MsoListContinue2CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue2CxSpLast, li.MsoListContinue2CxSpLast, div.MsoListContinue2CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue3, li.MsoListContinue3, div.MsoListContinue3
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue3CxSpFirst, li.MsoListContinue3CxSpFirst, div.MsoListContinue3CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue3CxSpMiddle, li.MsoListContinue3CxSpMiddle, div.MsoListContinue3CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue3CxSpLast, li.MsoListContinue3CxSpLast, div.MsoListContinue3CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue4, li.MsoListContinue4, div.MsoListContinue4
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue4CxSpFirst, li.MsoListContinue4CxSpFirst, div.MsoListContinue4CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue4CxSpMiddle, li.MsoListContinue4CxSpMiddle, div.MsoListContinue4CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue4CxSpLast, li.MsoListContinue4CxSpLast, div.MsoListContinue4CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:72.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue5, li.MsoListContinue5, div.MsoListContinue5
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue5CxSpFirst, li.MsoListContinue5CxSpFirst, div.MsoListContinue5CxSpFirst
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue5CxSpMiddle, li.MsoListContinue5CxSpMiddle, div.MsoListContinue5CxSpMiddle
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListContinue5CxSpLast, li.MsoListContinue5CxSpLast, div.MsoListContinue5CxSpLast
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:90.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoMessageHeader, li.MsoMessageHeader, div.MsoMessageHeader
	{mso-style-link:"メッセージ見出し \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:54.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:-54.0pt;
	background:#CCCCCC;
	border:none;
	padding:0mm;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoSubtitle, li.MsoSubtitle, div.MsoSubtitle
	{mso-style-link:"副題 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:12.0pt;
	margin-left:0mm;
	text-align:center;
	line-height:105%;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoSalutation, li.MsoSalutation, div.MsoSalutation
	{mso-style-link:"挨拶文 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoDate, li.MsoDate, div.MsoDate
	{mso-style-link:"日付 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyTextFirstIndent, li.MsoBodyTextFirstIndent, div.MsoBodyTextFirstIndent
	{mso-style-link:"本文字下げ \(文字\)";
	margin:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyTextFirstIndent2, li.MsoBodyTextFirstIndent2, div.MsoBodyTextFirstIndent2
	{mso-style-link:"本文字下げ 2 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	text-indent:18.0pt;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoNoteHeading, li.MsoNoteHeading, div.MsoNoteHeading
	{mso-style-link:"記 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyText2, li.MsoBodyText2, div.MsoBodyText2
	{mso-style-link:"本文 2 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:200%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyText3, li.MsoBodyText3, div.MsoBodyText3
	{mso-style-link:"本文 3 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyTextIndent2, li.MsoBodyTextIndent2, div.MsoBodyTextIndent2
	{mso-style-link:"本文インデント 2 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:200%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBodyTextIndent3, li.MsoBodyTextIndent3, div.MsoBodyTextIndent3
	{mso-style-link:"本文インデント 3 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:6.0pt;
	margin-left:18.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoBlockText, li.MsoBlockText, div.MsoBlockText
	{margin-top:0mm;
	margin-right:57.6pt;
	margin-bottom:8.0pt;
	margin-left:57.6pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	border:none;
	padding:0mm;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:#1F4E79;
	font-style:italic;}
a:link, span.MsoHyperlink
	{font-family:"Meiryo UI";
	color:#0563C1;
	text-decoration:underline;}
a:visited, span.MsoHyperlinkFollowed
	{font-family:"Meiryo UI";
	color:#954F72;
	text-decoration:underline;}
strong
	{color:windowtext;}
em
	{color:windowtext;}
p.MsoDocumentMap, li.MsoDocumentMap, div.MsoDocumentMap
	{mso-style-link:"見出しマップ \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoPlainText, li.MsoPlainText, div.MsoPlainText
	{mso-style-link:"書式なし \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoAutoSig, li.MsoAutoSig, div.MsoAutoSig
	{mso-style-link:"電子メール署名 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p
	{margin-right:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:#404040;}
acronym
	{font-family:"Meiryo UI";}
address
	{mso-style-link:"HTML アドレス \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-style:italic;}
cite
	{font-family:"Meiryo UI";}
code
	{font-family:"Meiryo UI";}
dfn
	{font-family:"Meiryo UI";}
kbd
	{font-family:"Meiryo UI";}
pre
	{mso-style-link:"HTML 書式付き \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
samp
	{font-family:"Meiryo UI";}
tt
	{font-family:"Meiryo UI";}
var
	{font-family:"Meiryo UI";}
p.MsoCommentSubject, li.MsoCommentSubject, div.MsoCommentSubject
	{mso-style-link:"コメント内容 \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-weight:bold;}
p.MsoAcetate, li.MsoAcetate, div.MsoAcetate
	{mso-style-link:"吹き出し \(文字\)";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
span.MsoPlaceholderText
	{font-family:"Meiryo UI";
	color:#595959;}
p.MsoNoSpacing, li.MsoNoSpacing, div.MsoNoSpacing
	{margin:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoRMPane, li.MsoRMPane, div.MsoRMPane
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoListParagraph, li.MsoListParagraph, div.MsoListParagraph
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:42.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoQuote, li.MsoQuote, div.MsoQuote
	{mso-style-link:"引用文 \(文字\)";
	margin-top:10.0pt;
	margin-right:43.2pt;
	margin-bottom:8.0pt;
	margin-left:43.2pt;
	text-align:center;
	line-height:110%;
	font-size:12.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	font-style:italic;}
p.MsoIntenseQuote, li.MsoIntenseQuote, div.MsoIntenseQuote
	{mso-style-link:"引用文 2 \(文字\)";
	margin-right:46.8pt;
	margin-bottom:12.0pt;
	margin-left:46.8pt;
	text-align:center;
	line-height:105%;
	font-size:13.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
span.MsoSubtleEmphasis
	{color:windowtext;
	font-style:italic;}
span.MsoIntenseEmphasis
	{color:windowtext;
	font-weight:bold;
	font-style:italic;}
span.MsoSubtleReference
	{font-variant:small-caps;
	color:windowtext;
	text-decoration:underline;}
span.MsoIntenseReference
	{font-variant:small-caps;
	color:windowtext;
	font-weight:bold;
	text-decoration:underline;}
span.MsoBookTitle
	{font-variant:small-caps;
	color:windowtext;
	font-weight:bold;}
p.MsoBibliography, li.MsoBibliography, div.MsoBibliography
	{margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
p.MsoTocHeading, li.MsoTocHeading, div.MsoTocHeading
	{margin-top:16.0pt;
	margin-right:0mm;
	margin-bottom:2.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-after:avoid;
	font-size:14.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;
	text-transform:uppercase;
	letter-spacing:.2pt;
	font-weight:bold;}
span.1
	{mso-style-name:"見出し 1 \(文字\)";
	mso-style-link:"見出し 1";
	font-family:"Calibri",sans-serif;
	text-transform:uppercase;
	letter-spacing:.2pt;
	font-weight:bold;}
span.a
	{mso-style-name:"ヘッダー \(文字\)";
	mso-style-link:ヘッダー;
	font-family:"Meiryo UI";
	color:#3B3838;}
span.a0
	{mso-style-name:"表題 \(文字\)";
	mso-style-link:表題;
	font-family:"Calibri",sans-serif;
	letter-spacing:-.35pt;
	font-weight:bold;}
span.a1
	{mso-style-name:"副題 \(文字\)";
	mso-style-link:副題;
	font-family:"Calibri",sans-serif;}
span.a2
	{mso-style-name:"フッター \(文字\)";
	mso-style-link:フッター;
	font-family:"Meiryo UI";}
span.2
	{mso-style-name:"見出し 2 \(文字\)";
	mso-style-link:"見出し 2";
	font-family:"Calibri",sans-serif;
	font-weight:bold;}
span.a3
	{mso-style-name:"吹き出し \(文字\)";
	mso-style-link:吹き出し;
	font-family:"Meiryo UI";}
span.a4
	{mso-style-name:"コメント文字列 \(文字\)";
	mso-style-link:コメント文字列;
	font-family:"Meiryo UI";}
span.a5
	{mso-style-name:"コメント内容 \(文字\)";
	mso-style-link:コメント内容;
	font-family:"Meiryo UI";
	font-weight:bold;}
p.1-, li.1-, div.1-
	{mso-style-name:"見出し 1 - 改ページ";
	margin-top:18.0pt;
	margin-right:0mm;
	margin-bottom:12.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-before:always;
	page-break-after:avoid;
	border:none;
	padding:0mm;
	font-size:26.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
p.1-CxSpFirst, li.1-CxSpFirst, div.1-CxSpFirst
	{mso-style-name:"見出し 1 - 改ページCxSpFirst";
	margin-top:18.0pt;
	margin-right:0mm;
	margin-bottom:0mm;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-before:always;
	page-break-after:avoid;
	border:none;
	padding:0mm;
	font-size:26.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
p.1-CxSpMiddle, li.1-CxSpMiddle, div.1-CxSpMiddle
	{mso-style-name:"見出し 1 - 改ページCxSpMiddle";
	margin:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-before:always;
	page-break-after:avoid;
	border:none;
	padding:0mm;
	font-size:26.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
p.1-CxSpLast, li.1-CxSpLast, div.1-CxSpLast
	{mso-style-name:"見出し 1 - 改ページCxSpLast";
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:12.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	page-break-before:always;
	page-break-after:avoid;
	border:none;
	padding:0mm;
	font-size:26.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
p.a6, li.a6, div.a6
	{mso-style-name:画像;
	margin-top:12.0pt;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:windowtext;}
span.a7
	{mso-style-name:"本文 \(文字\)";
	mso-style-link:本文;
	font-family:"Meiryo UI";}
span.20
	{mso-style-name:"本文 2 \(文字\)";
	mso-style-link:"本文 2";
	font-family:"Meiryo UI";}
span.3
	{mso-style-name:"本文 3 \(文字\)";
	mso-style-link:"本文 3";
	font-family:"Meiryo UI";}
span.a8
	{mso-style-name:"本文字下げ \(文字\)";
	mso-style-link:本文字下げ;
	font-family:"Meiryo UI";}
span.a9
	{mso-style-name:"本文インデント \(文字\)";
	mso-style-link:本文インデント;
	font-family:"Meiryo UI";}
span.21
	{mso-style-name:"本文字下げ 2 \(文字\)";
	mso-style-link:"本文字下げ 2";
	font-family:"Meiryo UI";}
span.22
	{mso-style-name:"本文インデント 2 \(文字\)";
	mso-style-link:"本文インデント 2";
	font-family:"Meiryo UI";}
span.30
	{mso-style-name:"本文インデント 3 \(文字\)";
	mso-style-link:"本文インデント 3";
	font-family:"Meiryo UI";}
span.aa
	{mso-style-name:"結語 \(文字\)";
	mso-style-link:結語;
	font-family:"Meiryo UI";}
span.ab
	{mso-style-name:"日付 \(文字\)";
	mso-style-link:日付;
	font-family:"Meiryo UI";}
span.ac
	{mso-style-name:"見出しマップ \(文字\)";
	mso-style-link:見出しマップ;
	font-family:"Meiryo UI";}
span.ad
	{mso-style-name:"電子メール署名 \(文字\)";
	mso-style-link:電子メール署名;
	font-family:"Meiryo UI";}
span.ae
	{mso-style-name:"文末脚注文字列 \(文字\)";
	mso-style-link:文末脚注文字列;
	font-family:"Meiryo UI";}
span.af
	{mso-style-name:"脚注文字列 \(文字\)";
	mso-style-link:脚注文字列;
	font-family:"Meiryo UI";}
span.31
	{mso-style-name:"見出し 3 \(文字\)";
	mso-style-link:"見出し 3";
	font-family:"Calibri",sans-serif;
	letter-spacing:.2pt;}
span.4
	{mso-style-name:"見出し 4 \(文字\)";
	mso-style-link:"見出し 4";
	font-family:"Calibri",sans-serif;
	font-style:italic;}
span.5
	{mso-style-name:"見出し 5 \(文字\)";
	mso-style-link:"見出し 5";
	font-family:"Calibri",sans-serif;
	font-weight:bold;}
span.6
	{mso-style-name:"見出し 6 \(文字\)";
	mso-style-link:"見出し 6";
	font-family:"Calibri",sans-serif;
	font-weight:bold;
	font-style:italic;}
span.7
	{mso-style-name:"見出し 7 \(文字\)";
	mso-style-link:"見出し 7";
	font-style:italic;}
span.8
	{mso-style-name:"見出し 8 \(文字\)";
	mso-style-link:"見出し 8";
	font-weight:bold;}
span.9
	{mso-style-name:"見出し 9 \(文字\)";
	mso-style-link:"見出し 9";
	font-style:italic;}
span.HTML
	{mso-style-name:"HTML アドレス \(文字\)";
	mso-style-link:"HTML アドレス";
	font-family:"Meiryo UI";
	font-style:italic;}
span.HTML0
	{mso-style-name:"HTML 書式付き \(文字\)";
	mso-style-link:"HTML 書式付き";
	font-family:"Meiryo UI";}
span.23
	{mso-style-name:"引用文 2 \(文字\)";
	mso-style-link:"引用文 2";
	font-family:"Calibri",sans-serif;}
span.af0
	{mso-style-name:"マクロ文字列 \(文字\)";
	mso-style-link:マクロ文字列;
	font-family:"Meiryo UI";}
span.af1
	{mso-style-name:"メッセージ見出し \(文字\)";
	mso-style-link:メッセージ見出し;
	font-family:"Meiryo UI";
	background:#CCCCCC;}
span.af2
	{mso-style-name:"記 \(文字\)";
	mso-style-link:記;
	font-family:"Meiryo UI";}
span.af3
	{mso-style-name:"書式なし \(文字\)";
	mso-style-link:書式なし;
	font-family:"Meiryo UI";}
span.af4
	{mso-style-name:"引用文 \(文字\)";
	mso-style-link:引用文;
	font-family:"Calibri",sans-serif;
	font-style:italic;}
span.af5
	{mso-style-name:"挨拶文 \(文字\)";
	mso-style-link:挨拶文;
	font-family:"Meiryo UI";}
span.af6
	{mso-style-name:"署名 \(文字\)";
	mso-style-link:署名;
	font-family:"Meiryo UI";}
span.10
	{mso-style-name:未解決のメンション1;
	font-family:"Meiryo UI";
	color:#605E5C;
	background:#E1DFDD;}
span.11
	{mso-style-name:メンション1;
	font-family:"Meiryo UI";
	color:#2B579A;
	background:#E1DFDD;}
p.af7, li.af7, div.af7
	{mso-style-name:定型句を試す;
	margin-top:0mm;
	margin-right:36.0pt;
	margin-bottom:8.0pt;
	margin-left:36.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:#595959;
	font-style:italic;}
p.af8, li.af8, div.af8
	{mso-style-name:引用符による強調;
	mso-style-link:引用符による強調の文字;
	margin-top:0mm;
	margin-right:0mm;
	margin-bottom:8.0pt;
	margin-left:0mm;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;
	font-size:11.0pt;
	font-family:"Calibri",sans-serif;
	color:#3B3838;}
span.af9
	{mso-style-name:"段落番号 \(文字\)";
	mso-style-link:段落番号;
	font-family:"Meiryo UI";
	color:#3B3838;}
span.afa
	{mso-style-name:引用符による強調の文字;
	mso-style-link:引用符による強調;
	font-family:"Meiryo UI";
	color:#3B3838;}
span.12
	{mso-style-name:ハッシュタグ1;
	font-family:"Meiryo UI";
	color:#2B579A;
	background:#E1DFDD;}
span.13
	{mso-style-name:"スマート ハイパーリンク1";
	font-family:"Meiryo UI";
	text-decoration:underline;}
.MsoChpDefault
	{font-size:11.0pt;
	font-family:"Calibri",sans-serif;}
.MsoPapDefault
	{margin-bottom:8.0pt;
	text-align:justify;
	text-justify:inter-ideograph;
	line-height:105%;}
 /* Page Definitions */
 @page WordSection1
	{size:595.3pt 841.9pt;
	margin:72.0pt 72.0pt 72.0pt 72.0pt;}
div.WordSection1
	{page:WordSection1;}
 /* List Definitions */
 ol
	{margin-bottom:0mm;}
ul
	{margin-bottom:0mm;}
-->
</style>

</head>

<body lang=JA link="#0563C1" vlink="#954F72" style='word-wrap:break-word;
line-break:strict'>

<div class=WordSection1>

<p class=MsoTitleCxSpFirst><a name="_Hlk73178102"></a><span lang=EN-US
style='font-size:28.0pt;font-family:"Meiryo UI"'>ROS2 Computer Vision</span></p>

<p class=MsoTitleCxSpMiddle><span style='font-size:28.0pt;font-family:"Meiryo UI"'>お勉強ロボット<span
lang=EN-US>(</span>その<span lang=EN-US>1)<span style='color:black'><br>
</span></span></span><span lang=EN-US style='font-size:36.0pt;font-weight:normal'><img
width=147 height=108 id="図 10"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image001.png"></span><span
lang=EN-US style='font-size:36.0pt'>&nbsp;</span></p>

<p class=MsoTitleCxSpLast><span lang=EN-US style='font-size:60.0pt;color:red'>R</span><span
lang=EN-US style='font-size:60.0pt'>2<span style='color:#00B050'>C</span><span
style='color:#0070C0'>V</span></span><a name="_Hlk487785372"></a></p>

<p class=MsoNormal><span style='font-size:14.0pt;line-height:105%;font-family:
"Meiryo UI"'>初心者のために、Python3、ROS2およびOpenCVの学習用ロボットを提案します。その1ではコンピュータ(RasPi4)とコンピュータビジョンの基礎を掲載します。</span></p>

<p class=MsoNormal><span lang=EN-US><img width=133 height=96 id="図 12"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image002.png"></span><span
style='font-family:メイリオ'>　</span><span lang=EN-US><img width=104 height=75
id="図 14" src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image003.png"></span><span
style='font-family:メイリオ'>　</span><span lang=EN-US><img width=86 height=63
id="図 22" src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image004.png"></span><span
style='font-family:メイリオ'>　</span><span lang=EN-US><img width=73 height=53
id="図 23" src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image005.png"></span><span
style='font-family:メイリオ'>　</span><span lang=EN-US><img width=53 height=38
id="図 24" src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image006.png"></span><span
style='font-family:メイリオ'>　</span><span lang=EN-US><img width=32 height=23
id="図 25" src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image007.png"></span></p>

<p class=MsoNormal align=right style='text-align:right'><span lang=EN-US><img
width=85 height=21 id="図 3"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image008.png"></span><span
style='font-family:メイリオ'>　　株式会社人口知能ロボット研究所</span></p>

<p class=MsoNormal>&nbsp;</p>

<p class=MsoTocHeading><span style='font-family:メイリオ'>目次</span></p>

<p class=MsoToc1><span lang=EN-US><a href="#_Toc80182852"><span
style='font-family:"Meiryo UI"'>1.R2CV</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>のベース</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182853"><span
style='font-family:"Meiryo UI"'>R2CV-</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>お勉強ロボットについて</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182854"><span
style='font-family:"Meiryo UI"'>RaspberyPi4</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>の準備</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182855"><span
style='font-family:"Meiryo UI"'>RasPi4</span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182856"><span
style='font-family:"Meiryo UI"'>SD</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>カード</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182857"><span
style='font-family:"Meiryo UI"'>RasPi</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>電源ハット 5V</span></span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>電源/RS485/TTL</span></span><span
style='color:windowtext;display:none;text-decoration:none'>. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182858"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>ディスプレイ/HDMI</span></span><span
lang=EN-US style='font-family:"Meiryo UI"'><span lang=EN-US>ケーブル</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182859"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>キーボード・マウス</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182860"><span
style='font-family:"Meiryo UI"'>USB</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>ステレオカメラ</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182861"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>バッテリー</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182862"><span
style='font-family:"Meiryo UI"'>WiFi</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>ルーター</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc1><span lang=EN-US><a href="#_Toc80182863"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>2.RasPi4 SD</span></span><span
lang=EN-US style='font-family:"Meiryo UI"'><span lang=EN-US>カードの作り方</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182864"><span
style='font-family:"Meiryo UI"'>RaspberyPi4</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のEEPROM</span></span><span
lang=EN-US style='font-family:"Meiryo UI"'><span lang=EN-US>のアップデート</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182865"><span
style='font-family:"Meiryo UI"'>Raspberry Pi OS</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のinstall</span></span><span
style='color:windowtext;display:none;text-decoration:none'> </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182866"><span
style='font-family:"Meiryo UI"'>EEPROM</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>のアップデート</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182867"><span
style='font-family:"Meiryo UI"'>Ubuntu20.04LTS</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のインストール</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc1><span lang=EN-US><a href="#_Toc80182868"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>3.</span></span><span
lang=EN-US style='font-family:"Meiryo UI"'><span lang=EN-US>ネットワークなど開発環境の準備</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182869"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>ネットワーク接続</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182870"><span
style='font-family:"Meiryo UI"'>Windows</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>リモートデスクトップ接続</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc1><span lang=EN-US><a href="#_Toc80182871"><span
style='font-family:"Meiryo UI"'>4.Open CV4</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>について</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182872"><span
style='font-family:"Meiryo UI"'>OpenCV</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>とは</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182873"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>インストールの手順</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182874"><span
style='font-family:"Meiryo UI"'>SwapFil</span><span style='color:windowtext;
display:none;text-decoration:none'> </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182875"><span
style='font-family:"Meiryo UI"'>opencv4</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のインストール</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182876"><span
style='font-family:"Meiryo UI"'>opencv-python</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のインストール</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182877"><span
style='font-family:"Meiryo UI"'>OpenCV</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>の動作確認</span></span><span style='color:windowtext;
display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182878"><span
style='font-family:"Meiryo UI"'>USB</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>カメラの接続</span></span><span style='color:windowtext;
display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182879"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>カメラ画像の取り込み</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182880"><span
style='font-family:"Meiryo UI"'>Open CV</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のサンプルプログラム</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc1><span lang=EN-US><a href="#_Toc80182881"><span
style='font-family:"Meiryo UI"'>5.</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>画像処理</span></span><span style='color:windowtext;
display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182882"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>色認識</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182883"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>ステレオカメラ</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182884"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>深層学習推論</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182885"><span
style='font-family:"Meiryo UI"'>Yolo v3</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>の推論サンプル</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc1><span lang=EN-US><a href="#_Toc80182886"><span
style='font-family:"Meiryo UI"'>6.ROS2</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>について</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182887"><span
style='font-family:"Meiryo UI"'>ROS2 Foxy</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>のインストール</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182888"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>参考サイト</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182889"><span
style='font-family:"Meiryo UI"'>ROS2 Foxy</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>デスクトップのインストール</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182890"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>ワークスペースの作成</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182891"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>パッケージの作成</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182892"><span
style='font-family:"Meiryo UI"'>ROS</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>について</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182893"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>なぜROS</span></span><span
lang=EN-US style='font-family:"Meiryo UI"'><span lang=EN-US>か?</span></span><span
style='color:windowtext;display:none;text-decoration:none'>. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182894"><span
style='font-family:"Meiryo UI"'>ROS</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>の構造</span></span><span style='color:windowtext;
display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182895"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>分散開発</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc2><span lang=EN-US><a href="#_Toc80182896"><span
style='font-family:"Meiryo UI"'>ROS2</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>を体感する。</span></span><span style='color:windowtext;
display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182897"><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>・カメラ画像の取り込み</span></span><span
style='color:windowtext;display:none;text-decoration:none'>... </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182898"><span
style='font-family:"Meiryo UI"'>rqt</span><span lang=EN-US style='font-family:
"Meiryo UI"'><span lang=EN-US>でカメラ画像を表示します。</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoToc3><span lang=EN-US><a href="#_Toc80182899"><span
style='font-family:"Meiryo UI"'>rosbag2</span><span lang=EN-US
style='font-family:"Meiryo UI"'><span lang=EN-US>で録画してみよう。</span></span><span
style='color:windowtext;display:none;text-decoration:none'>.. </span><span
style='color:windowtext;display:none;text-decoration:none'>1</span></a></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h1><a name="_Toc80182852"><span lang=EN-US style='font-size:26.0pt;line-height:
105%;font-family:"Meiryo UI";color:#3B3838'>1.R2CV</span></a><span
style='font-size:26.0pt;line-height:105%;font-family:"Meiryo UI";color:#3B3838'>のベース</span></h1>

<h2><a name="_Toc80182853"><span lang=EN-US style='font-family:"Meiryo UI"'>R2CV-</span></a><span
style='font-family:"Meiryo UI"'>お勉強ロボットについて</span></h2>

<p class=MsoNormal><span lang=EN-US>-RasPi4+Ubuntu20.04LTS+Python3+ROS2-Foxy+OpenCV4</span><span
style='font-family:メイリオ'>を使用します。</span></p>

<p class=MsoNormal><span lang=EN-US>-</span><span style='font-family:メイリオ'>まずは足回りは</span><span
lang=EN-US>2Wheel</span><span style='font-family:メイリオ'>ステアリング方式で進めます。</span></p>

<p class=MsoNormal><span lang=EN-US>-</span><span style='font-family:メイリオ'>将来ロボットアームや</span><span
lang=EN-US>2</span><span style='font-family:メイリオ'>足歩行ロボットへ展開します。</span></p>

<p class=MsoNormal align=left style='text-align:left'><span lang=EN-US><img
width=167 height=220 id="図 19"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image009.png"></span></p>

<p class=MsoNormal align=center style='text-align:center'><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182854"><span lang=EN-US style='font-family:"Meiryo UI"'>RaspberyPi4</span></a><span
style='font-family:"Meiryo UI"'>の準備</span></h2>

<h3><a name="_Toc80182855"><span class=MsoIntenseEmphasis><span lang=EN-US
style='font-family:"Meiryo UI";font-weight:normal;font-style:normal'>RasPi4</span></span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>メモリーは出来れば</span><span
lang=EN-US>8GByte</span><span style='font-family:メイリオ'>のものを準備しましょう。</span></p>

<p class=MsoNormal><span lang=EN-US><img width=179 height=135 id="図 30"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image010.jpg"></span><span
style='font-family:メイリオ'>　</span><span lang=EN-US><img width=220 height=133
id="図 2" src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image011.png"></span></p>

<h3><a name="_Toc80182856"><span class=MsoIntenseEmphasis><span lang=EN-US
style='font-family:"Meiryo UI";font-weight:normal;font-style:normal'>SD</span></span></a><span
class=MsoIntenseEmphasis><span style='font-family:"Meiryo UI";font-weight:normal;
font-style:normal'>カード</span></span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>高速のもので</span><span
lang=EN-US>32Gbyte</span><span style='font-family:メイリオ'>以上のものを使用します。同じ</span><span
lang=EN-US>32Gbyte</span><span style='font-family:メイリオ'>でも容量が異なるので、コピーするときには注意してください。</span></p>

<p class=MsoNormal><span lang=EN-US><img width=95 height=59 id="図 9"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image012.png"></span></p>

<p class=MsoNormal><span lang=EN-US style='background:yellow'>RasPi4+Ubuntu20.04LTS+Python3+ROS2-Foxy+OpenCV4</span><span
style='font-family:メイリオ;background:yellow'>をインストールした</span><span lang=EN-US
style='background:yellow'>SD</span><span style='font-family:メイリオ;background:
yellow'>カードのイメージファイルは以下よりダウンロードできます。</span></p>

<p class=MsoNormal><span lang=EN-US><a
href="http://arrc.jp/auto/r2cv_20210816.img"><span style='background:yellow'>http://arrc.jp/auto/r2cv_20210816.img</span></a></span></p>

<p class=MsoNormal><span style='font-family:メイリオ;background:yellow'>ユーザー</span><span
lang=EN-US style='background:yellow'>:ubuntu</span></p>

<p class=MsoNormal><span style='font-family:メイリオ;background:yellow'>パスワード</span><span
lang=EN-US style='background:yellow'>:airrcrobo</span></p>

<h3><a name="_Toc80182857"><span lang=EN-US style='font-family:"Meiryo UI"'>RasPi</span></a><span
style='font-family:"Meiryo UI"'>電源ハット <span lang=EN-US>5V</span>電源<span
lang=EN-US>/RS485/TTL</span></span></h3>

<p class=MsoNormal><span lang=EN-US style='font-size:10.5pt;line-height:105%'>DXHAT------
</span><span style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>（株）ベストテクノロジー</span></p>

<p class=MsoNormal><span lang=EN-US><a
href="http://www.besttechnology.co.jp/modules/knowledge/?DXHAT#c66a2597"><span
style='font-size:10.5pt;line-height:105%'>http://www.besttechnology.co.jp/modules/knowledge/?DXHAT#c66a2597</span></a></span></p>

<p class=MsoNormal><span lang=EN-US style='font-size:10.5pt;line-height:105%'><img
border=0 width=331 height=231 id="図 20"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image013.jpg"></span></p>

<p class=MsoNormal><span lang=EN-US style='font-size:10.5pt;line-height:105%'>DXHAT</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>は</span><span
lang=EN-US style='font-size:10.5pt;line-height:105%'>Raspberry Pi 4</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>用の電源</span><span
lang=EN-US style='font-size:10.5pt;line-height:105%'>HAT</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>です。</span><span
lang=EN-US style='font-size:10.5pt;line-height:105%'>Raspberry Pi</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>への電源供給は外付けのプッシュスイッチによって</span><span
lang=EN-US style='font-size:10.5pt;line-height:105%'>ON/OFF</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>する事ができ、更にサーボモータなどをコントロールする</span><span
lang=EN-US style='font-size:10.5pt;line-height:105%'>RS-485</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>と</span><span
lang=EN-US style='font-size:10.5pt;line-height:105%'>TTL I/F</span><span
style='font-size:10.5pt;line-height:105%;font-family:メイリオ'>を装備しています。</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182858"><span style='font-family:"Meiryo UI"'>ディスプレイ<span
lang=EN-US>/HDMI</span>ケーブル</span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>ディスプレイはセットアップの時だけ使用するので何でも良いです。ただし</span><span
lang=EN-US>HDMI</span><span style='font-family:メイリオ'>ケーブルはシールドがしっかりしているものを使いましょう。</span><span
lang=EN-US>WiFi</span><span style='font-family:メイリオ'>接続トラブルの原因となります。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=89 height=89 id="図 13"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image014.png"></span></p>

<h3><a name="_Toc80182859"><span style='font-family:"Meiryo UI"'>キーボード・マウス</span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>何でも良いです。セットアップのときに使用します。</span></p>

<h3><a name="_Toc80182860"><span lang=EN-US style='font-family:"Meiryo UI"'>USB</span></a><span
style='font-family:"Meiryo UI"'>ステレオカメラ</span><span lang=EN-US
style='font-family:"Meiryo UI"'>&nbsp;&nbsp; <a name="_Hlk80016688"></a></span></h3>

<p class=MsoNormal><span lang=EN-US>&nbsp; ------ amazon</span><span
style='font-family:メイリオ'>で購入</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=133 height=89 id="図 6"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image015.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182861"><span style='font-family:"Meiryo UI"'>バッテリー</span></a><span
style='font-family:"Meiryo UI"'> </span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>ここでは</span><span lang=EN-US>7.4V</span><span
style='font-family:メイリオ'>で使用していますが、使用するサーボモータの電圧仕様に合ったものを使用してください。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=178 height=107 id="図 5"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image016.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182862"><span lang=EN-US style='font-family:"Meiryo UI"'>WiFi</span></a><span
style='font-family:"Meiryo UI"'>ルーター</span></h3>

<p class=MsoNormal style='text-indent:11.0pt'><span style='font-family:メイリオ'>何でも良いです。</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h1><a name="_Hlk73173570"></a><a name="_Toc80182863"><span style='font-size:
26.0pt;line-height:105%;font-family:"Meiryo UI";color:#3B3838'>2.RasPi4 SDカードの作り方</span></a></h1>

<h2><a name="_Toc80182864"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>RaspberyPi4</span></a><span style='font-size:
16.0pt;line-height:105%;font-family:"Meiryo UI"'>の<span lang=EN-US>EEPROM</span>のアップデート</span></h2>

<p class=MsoNormal><span style='font-family:メイリオ'>以下の手順に従い</span><span
lang=EN-US>RasPi4</span><span style='font-family:メイリオ'>の</span><span
lang=EN-US>EEPROM</span><span style='font-family:メイリオ'>の内容を最新版にアップデートします。ディスプレイ、マウス、キーボード、</span><span
lang=EN-US>LAN</span><span style='font-family:メイリオ'>ケーブルを接続しておいてください。</span></p>

<h3><a name="_Toc80182865"></a><a name="_Hlk74818172"><span lang=EN-US
style='font-family:"Meiryo UI"'>Raspberry Pi </span></a><span lang=EN-US
style='font-family:"Meiryo UI"'>OS</span><span style='font-family:"Meiryo UI"'>の<span
lang=EN-US>install</span></span></h3>

<p class=MsoNormal><span lang=EN-US>&nbsp;&nbsp; </span><span style='font-family:
メイリオ'>以下のサイトより</span><span lang=EN-US>Raspberry Pi imager</span><span
style='font-family:メイリオ'>をインストールします。</span></p>

<p class=MsoNormal><span lang=EN-US>Raspberry Pi imager</span><span
style='font-family:メイリオ'>を起動し、</span><span lang=EN-US>ERACE</span><span
style='font-family:メイリオ'>を選択し、</span><span lang=EN-US>SD</span><span
style='font-family:メイリオ'>カードをフォーマットします。続いて、</span><a name="_Hlk74818096"><span
lang=EN-US>Raspberry Pi OS</span></a><span style='font-family:メイリオ'>を</span><span
lang=EN-US>SD</span><span style='font-family:メイリオ'>カードに書き込みます。</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span><span style='font-family:メイリオ'>参考サイト</span><span
lang=EN-US>: </span><a href="https://www.raspberrypi.org/downloads/"><span
lang=EN-US style='font-family:"Meiryo UI"'>https://www.raspberrypi.org/downloads/</span></a></p>

<p class=MsoNormal style='text-indent:66.0pt'><a
href="https://www.raspberrypi.org/software/"><span lang=EN-US style='font-family:
"Meiryo UI"'>https://www.raspberrypi.org/software/</span></a></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182866"><span lang=EN-US style='font-family:"Meiryo UI"'>EEPROM</span></a><span
style='font-family:"Meiryo UI"'>のアップデート</span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>参考サイト</span><span lang=EN-US>:
</span></p>

<p class=MsoNormal><a
href="https://www.raspberrypi.org/documentation/hardware/raspberrypi/booteeprom.md"><span
lang=EN-US style='font-family:"Meiryo UI"'>https://www.raspberrypi.org/documentation/hardware/raspberrypi/booteeprom.md</span></a></p>

<p class=MsoNormal><span style='font-family:メイリオ'>以下のコマンドを実行して</span><span
lang=EN-US>EEPROM</span><span style='font-family:メイリオ'>をアップデートします。</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt-get update &amp;&amp; sudo
apt-get dist-upgrade -y</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo rpi-update</span></p>

<p class=MsoNormal><span lang=EN-US>$ reboot</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo rpi-eeprom-update -a</span></p>

<p class=MsoNormal><span lang=EN-US>$ reboot</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182867"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>Ubuntu20.04LTS</span></a><span style='font-size:
16.0pt;line-height:105%;font-family:"Meiryo UI"'>のインストール</span></h2>

<p class=MsoNormal><span lang=EN-US>Raspberry Pi imager</span><span
style='font-family:メイリオ'>から</span><span lang=EN-US>Ubuntu Server 20.04.2LTS
64-bit</span><span style='font-family:メイリオ'>版を</span><span lang=EN-US>SD</span><span
style='font-family:メイリオ'>カードに書き込みます。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=325 height=219 id="図 1"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image017.jpg"></span></p>

<p class=MsoNormal><span lang=EN-US>SD</span><span style='font-family:メイリオ'>カードを</span><span
lang=EN-US>Raspi4</span><span style='font-family:メイリオ'>にセットし起動します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>アカウント名「</span><span
lang=EN-US>ubuntu</span><span lang=EN-US style='font-family:"Tahoma",sans-serif'>&#8288;</span><span
style='font-family:メイリオ'>」</span><span lang=EN-US style='font-family:"Tahoma",sans-serif'>&#8288;</span><span
style='font-family:メイリオ'>，パスワード「</span><span lang=EN-US>ubuntu</span><span
style='font-family:メイリオ'>」でログインします。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>まずは以下を実行しアップデートしておきます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt update</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt full-upgrade -y</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>次にサーバー版をデスクトップ版に変更します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>ここでは</span><span lang=EN-US>Desktopify</span><span
style='font-family:メイリオ'>を使用します。サーバー版の</span><span lang=EN-US>Ubuntu 20.04 LTS</span><span
style='font-family:メイリオ'>がインストールされた</span><span lang=EN-US>Raspberry Pi</span><span
style='font-family:メイリオ'>上で実行することでデスクトップ環境をインストールしてくれます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ git clone
https://github.com/wimpysworld/desktopify.git</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd desktopify</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo ./desktopify --de ubuntu</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo reboot</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>以上でディスクトップ環境が完成です。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>「設定」にて言語や</span><span
lang=EN-US>WiFi</span><span style='font-family:メイリオ'>、ディスプレイなどの使用環境を設定してください。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>その他、以下のサイトをご参照ください。</span> </p>

<p class=MsoNormal><span style='font-family:メイリオ'>参考サイト</span><span lang=EN-US>:
</span><a href="https://gihyo.jp/admin/serial/01/ubuntu-recipe/0624?page=1"><span
lang=EN-US style='font-family:"Meiryo UI"'>https://gihyo.jp/admin/serial/01/ubuntu-recipe/0624?page=1</span></a></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h1><a name="_Hlk73174372"></a><a name="_Toc80182868"><span style='font-size:
26.0pt;line-height:105%;font-family:"Meiryo UI";color:#3B3838'>3.ネットワークなど開発環境の準備</span></a></h1>

<h2><a name="_Toc80182869"><span style='font-size:16.0pt;line-height:105%;
font-family:"Meiryo UI"'>ネットワーク接続</span></a></h2>

<p class=MsoNormal><span style='font-family:メイリオ'>マウス、キーボード、ディスプレイを接続して、</span><span
lang=EN-US>WiFi</span><span style='font-family:メイリオ'>によるネットワークに接続を行います。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=247 height=199 id="図 4"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image018.jpg"></span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>右上のボタンから</span><span
lang=EN-US>WiFi</span><span style='font-family:メイリオ'>を選んで接続してください。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>以下を実行し</span><span
lang=EN-US>net-tool</span><span style='font-family:メイリオ'>をインストールすれば</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudu apt install net-tool</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>下記コマンドで</span><span
lang=EN-US>IP</span><span style='font-family:メイリオ'>アドレスを確認できます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ ifconfig</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>で</span><span lang=EN-US>IP</span><span
style='font-family:メイリオ'>が表示されます。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>この</span><span lang=EN-US>IP</span><span
style='font-family:メイリオ'>アドレスにリモートデスクトップから接続します。</span></p>

<h2><a name="_Toc80182870"><span lang=EN-US style='font-family:"Meiryo UI"'>Windows</span></a><span
style='font-family:"Meiryo UI"'>リモートデスクトップ接続</span></h2>

<p class=MsoNormal><span lang=EN-US>Windows</span><span style='font-family:
メイリオ'>から</span><span lang=EN-US>RasPi4</span><span style='font-family:メイリオ'>にリモートデスクトップで接続します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>まず</span><span lang=EN-US>Xrdp
</span><span style='font-family:メイリオ'>サーバーを</span><span lang=EN-US>RasPi4</span><span
style='font-family:メイリオ'>にインストールして起動します。</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt -y install xrdp
tigervnc-standalone-server</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo systemctl enable xrdp</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>さらに「設定」にてディスプレイの共有を許可しておいてください。</span></p>

<p class=MsoNormal><span lang=EN-US>Windows</span><span style='font-family:
メイリオ'>のリモートデスクトップから</span><span lang=EN-US>IP</span><span style='font-family:
メイリオ'>アドレスを指定して接続します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>参考サイト</span><span lang=EN-US>:</span></p>

<p class=MsoNormal><span lang=EN-US><a
href="https://www.server-world.info/query?os=Ubuntu_20.04&amp;p=desktop&amp;f=6"><span
style='font-family:"Meiryo UI"'>https://www.server-world.info/query?os=Ubuntu_20.04&amp;p=desktop&amp;f=6</span></a></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h1><a name="_Toc80182871"><span lang=EN-US style='font-size:26.0pt;line-height:
105%;font-family:"Meiryo UI";color:#3B3838'>4.Open CV4</span></a><span
style='font-size:26.0pt;line-height:105%;font-family:"Meiryo UI";color:#3B3838'>について</span></h1>

<h2><a name="_Toc80182872"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>OpenCV</span></a><span style='font-size:16.0pt;
line-height:105%;font-family:"Meiryo UI"'>とは</span></h2>

<p class=MsoNormal><span lang=EN-US>OpenCV</span><span style='font-family:メイリオ'>はオープンソースの画像処理や機械学習のソフトウェアーのライブラリーです。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>以下のサイトをご参照ください。</span></p>

<p class=MsoNormal><span lang=EN-US><a href="https://opencv.org/"><span
style='font-family:"Meiryo UI"'>https://opencv.org/</span></a></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182873"><span style='font-size:16.0pt;line-height:105%;
font-family:"Meiryo UI"'>インストールの手順</span></a></h2>

<h3><a name="_Toc80182874"><span lang=EN-US style='font-family:"Meiryo UI"'>SwapFil</span></a></h3>

<p class=MsoNormal><span lang=EN-US>OpenCV</span><span style='font-family:メイリオ'>をコンパイルするときに大量のメモリーを使いますので、メモリーが</span><span
lang=EN-US>4Gbyte</span><span style='font-family:メイリオ'>以下の場合はディスクをメモリーとして使う</span><span
lang=EN-US>Swapfile</span><span style='font-family:メイリオ'>をインストールします。</span></p>

<p class=MsoNormal><span lang=EN-US>$ git clone https://github.com/JetsonHacksNano/installSwapfile</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd installSwapfile</span></p>

<p class=MsoNormal><span lang=EN-US>$ ./installSwapfile.sh</span></p>

<h3><a name="_Toc80182875"><span lang=EN-US style='font-family:"Meiryo UI"'>opencv4</span></a><span
style='font-family:"Meiryo UI"'>のインストール</span></h3>

<p class=MsoNormal><span lang=EN-US>Open cv4.*</span><span style='font-family:
メイリオ'>の最新版をインストールします、</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>インストールスクリプト</span><span
lang=EN-US>install-opencv.sh</span><span style='font-family:メイリオ'>をダウンロードして実行してください。</span></p>

<p class=MsoNormal><span lang=EN-US>$ wget --no-check-certificate
https://raw.githubusercontent.com/milq/milq/master/scripts/bash/install-opencv.sh</span></p>

<p class=MsoNormal><span lang=EN-US>$ chmod +x install-opencv.sh</span></p>

<p class=MsoNormal><span lang=EN-US>$ ./install-opencv.sh</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>コンパイルには数時間かかります。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>参考サイト</span><span lang=EN-US>:
</span><span lang=EN-US><a
href="http://milq.github.io/install-opencv-ubuntu-debian"><span
style='font-family:"Meiryo UI"'>http://milq.github.io/install-opencv-ubuntu-debian</span></a></span></p>

<h3><a name="_Toc80182876"><span lang=EN-US>opencv-python</span></a><span
style='font-family:メイリオ'>のインストール</span></h3>

<p class=MsoNormal><span lang=EN-US>$ sudo apt install python3-pip</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo pip install opencv-python</span></p>

<h2><a name="_Toc80182877"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>OpenCV</span></a><span style='font-size:16.0pt;
line-height:105%;font-family:"Meiryo UI"'>の動作確認</span></h2>

<h3><a name="_Toc80182878"><span lang=EN-US style='font-family:"Meiryo UI"'>USB</span></a><span
style='font-family:"Meiryo UI"'>カメラの接続</span></h3>

<p class=MsoNormal><span lang=EN-US>Raspi4</span><span style='font-family:メイリオ'>に</span><span
lang=EN-US>USB</span><span style='font-family:メイリオ'>カメラを接続します。</span></p>

<p class=MsoNormal><span lang=EN-US>$ ls /dev/video*</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>でカメラの接続を確認できます。</span></p>

<h3><a name="_Toc80182879"><span style='font-family:"Meiryo UI"'>カメラ画像の取り込み</span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>まず</span><span lang=EN-US>$ home</span><span
style='font-family:メイリオ'>ディレクトリーに</span><span lang=EN-US>gitHub</span><span
style='font-family:メイリオ'>の</span><span lang=EN-US>airrc</span><span
style='font-family:メイリオ'>フォルダーのコピー作成します。</span><span lang=EN-US>cam_sample.py</span><span
style='font-family:メイリオ'>を実行します。</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd airrc</span></p>

<p class=MsoNormal><span lang=EN-US>$ python3 <a name="_Hlk75011941">cam_sample.py</a></span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>と入力してください。画面にカメラの画像が表示されれば</span><span
lang=EN-US>Python3</span><span style='font-family:メイリオ'>と</span><span
lang=EN-US>OpenCV</span><span style='font-family:メイリオ'>は動作しています。</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182880"><span lang=EN-US style='font-family:"Meiryo UI"'>Open
CV</span></a><span style='font-family:"Meiryo UI"'>のサンプルプログラム</span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>以下のディレクトリーに</span><span
lang=EN-US>Python</span><span style='font-family:メイリオ'>のサンプルプログラムがあります。画像処理に興味のある方はいろいろ使ってみましょう。</span></p>

<p class=MsoNormal><span lang=EN-US>ubuntu@ubuntu:~/<a name="_Hlk74853993">OpenCV/</a>samples/python$</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h1><a name="_Toc80182881"><span lang=EN-US style='font-size:24.0pt;line-height:
105%;font-family:"Meiryo UI"'>5.</span></a><span style='font-size:24.0pt;
line-height:105%;font-family:"Meiryo UI"'>画像処理</span></h1>

<h2><a name="_Toc80182882"><span style='font-size:16.0pt;line-height:105%;
font-family:メイリオ'>色認識</span></a></h2>

<p class=MsoNormal><span style='font-family:メイリオ'>・<a name="_Hlk73184495">色認識　</a></span><span
lang=EN-US>HSV</span><span style='font-family:メイリオ'>が人の感覚と合うので色認識においては使用されます。探す色の</span><span
lang=EN-US>HSV</span><span style='font-family:メイリオ'>値にフィルターをかけます。次のプログラムは</span><span
lang=EN-US>HSV</span><span style='font-family:メイリオ'>の</span><span lang=EN-US>Hue</span><span
style='font-family:メイリオ'>を数値化するプログラムです。</span></p>

<p class=MsoNormal><span lang=EN-US>USB</span><span style='font-family:メイリオ'>カメラをセットし、プログラムのあるディレクトリーにて以下を実行してください。</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd airrc</span></p>

<p class=MsoNormal><span lang=EN-US>$ python3 hsv_color_set.py</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>画面にカメラ画像と</span><span
lang=EN-US>Hue Bar</span><span style='font-family:メイリオ'>が表示されます。緑の線の上をタッチすると</span><span
lang=EN-US>Hue</span><span style='font-family:メイリオ'>の下限値、緑線の下をタッチすると上限をセットできます。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>その結果がカメラ画像に表示されます。ここで設定した</span><span
lang=EN-US>Hue</span><span style='font-family:メイリオ'>の上下限を使えば色認識ができます。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=237 height=265 id="図 11"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image019.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182883"><span style='font-size:16.0pt;line-height:105%;
font-family:"Meiryo UI"'>ステレオカメラ</span></a></h2>

<p class=MsoNormal><span style='font-family:メイリオ'>ステレオカメラを使うと</span><span
lang=EN-US>2</span><span style='font-family:メイリオ'>つのカメラの視差から距離を求めることができます。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>視差を求めるにはステレオ画像マッチング手法を使います。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>マッチング手法には</span><span
lang=EN-US>SGM</span><span style='font-family:メイリオ'>（</span><span lang=EN-US>Semi
Global Matching</span><span style='font-family:メイリオ'>）方式、</span><span
lang=EN-US>SAD</span><span style='font-family:メイリオ'>（</span><span lang=EN-US>Sum
of Absolute Difference</span><span style='font-family:メイリオ'>）方式などがありますが、変化のないところではマッチングできないため、赤外線や可視光でパターン照射を行っているものがあります。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=234 height=228 id="図 8"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image020.png"></span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>ここでは注目点を探してその点に対して視差から距離を求めます。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>サンプルプログラムでは注目点として赤色を認識してその距離を求めます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd airrc</span></p>

<p class=MsoNormal><span lang=EN-US>$ python3 stereo_color.py</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>このプログラムでは赤色のものまでの座標と距離を計算します。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=394 height=297 id="図 18"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image021.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182884"><span style='font-size:16.0pt;line-height:105%;
font-family:"Meiryo UI"'>深層学習推論</span></a></h2>

<p class=MsoNormal><span style='font-family:メイリオ'>画像の深層学習には画像分類</span><span
lang=EN-US>/</span><span style='font-family:メイリオ'>物体認識</span><span lang=EN-US>/</span><span
style='font-family:メイリオ'>セグメンテーションがあります。</span></p>

<p class=MsoNormal><b><span style='font-family:メイリオ'>画像分類</span></b><b><span
lang=EN-US>(Classification)</span></b></p>

<p class=MsoNormal style='text-indent:11.0pt'><span style='font-family:メイリオ'>画像分類するアルゴリズムです。</span></p>

<p class=MsoNormal><b><span style='font-family:メイリオ'>物体認識</span></b><b><span
lang=EN-US>(Object detection)</span></b></p>

<p class=MsoNormal style='text-indent:11.0pt'><span lang=EN-US>1: </span><span
style='font-family:メイリオ'>物体領域候補の抽出</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>　</span><span lang=EN-US>2: </span><span
style='font-family:メイリオ'>物体領域候補の物体認識</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>　</span><span lang=EN-US>3: </span><span
style='font-family:メイリオ'>検出領域の絞り込み</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>を行い物体とその位置を認識します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>以下の手法があります。</span></p>

<p class=MsoNormal><b><span lang=EN-US>SSD (Single Shot Multibox Detector)</span></b></p>

<p class=MsoNormal style='text-indent:5.5pt'><span lang=EN-US>&nbsp;SSD </span><span
style='font-family:メイリオ'>は深層学習ベースの物体検出アルゴリズム，物体候補領域の生成と分類を同時に学習・実行することが可能です。</span></p>

<p class=MsoNormal><b><span lang=EN-US>YOLO(You only look once)</span></b></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;&nbsp; YOLO </span><span
style='font-family:メイリオ'>では領域候補の抽出するのではなく直接的に物体検出をしようというものです。</span></p>

<p class=MsoNormal><b><span style='font-family:メイリオ'>領域分割</span></b><b><span
lang=EN-US>(Segmentation)</span></b></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span><span style='font-family:メイリオ'>画像の領域を分割するタスクを</span><span
lang=EN-US>Segmentation(</span><a name="_Hlk80172661"><span style='font-family:
メイリオ'>領域分割</span></a><span lang=EN-US>)</span><span style='font-family:メイリオ'>と呼び、</span><span
lang=EN-US>Semantic Segmentation</span><span style='font-family:メイリオ'>は「何が写っているか」で画像領域を分割するタスクのことを指す。</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182885"><span lang=EN-US>Yolo v3</span></a><span
style='font-family:メイリオ'>の推論サンプル</span></h3>

<p class=MsoNormal><span style='font-family:メイリオ;background:yellow'>カメラを接続し</span><span
lang=EN-US style='background:yellow'>airrc/auto_dl</span><span
style='font-family:メイリオ;background:yellow'>フォルダに移り、以下のプログラムを実行すると</span><span
lang=EN-US style='background:yellow'>ROBO-ONE auto</span><span
style='font-family:メイリオ;background:yellow'>リモートで使用するダミーロボットとグリーンボトルを認識できます。</span></p>

<p class=MsoNormal><span lang=EN-US style='background:yellow'>$ cd airrc/auto_dl</span></p>

<p class=MsoNormal><span lang=EN-US style='background:yellow'>$ pythin3
auto_dl.py</span></p>

<p class=MsoNormal align=left style='text-align:left'><span lang=EN-US><img
border=0 width=380 height=214 id="図 7"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image022.png"></span></p>

<p class=MsoNormal align=left style='text-align:left'><span lang=EN-US>&nbsp;</span></p>

<h1><a name="_Toc80182886"><span lang=EN-US style='font-size:26.0pt;line-height:
105%;font-family:"Meiryo UI";color:#3B3838'>6.ROS2</span></a><span
style='font-size:26.0pt;line-height:105%;font-family:"Meiryo UI";color:#3B3838'>について</span></h1>

<h2><a name="_Toc80182887"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>ROS2 Foxy</span></a><span style='font-size:16.0pt;
line-height:105%;font-family:"Meiryo UI"'>のインストール</span></h2>

<h3><a name="_Toc80182888"><span style='font-family:"Meiryo UI"'>参考サイト</span></a></h3>

<p class=MsoNormal><span lang=EN-US><a
href="https://index.ros.org/doc/ros2/Installation/">https://index.ros.org/doc/ros2/Installation/</a></span></p>

<h3><a name="_Toc80182889"><span lang=EN-US style='font-family:"Meiryo UI"'>ROS2
Foxy</span></a><span style='font-family:"Meiryo UI"'>デスクトップのインストール</span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>以下のコマンドを実行すると</span><span
lang=EN-US>ROS2 Foxy Desktop</span><span style='font-family:メイリオ'>をインストールできます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt update</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt install curl gnupg2 lsb-release</span></p>

<p class=MsoNormal><span lang=EN-US>$ curl -s
https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key
add -</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo sh -c 'echo &quot;deb
[arch=amd64,arm64] http://packages.ros.org/ros2/ubuntu `lsb_release -cs`
main&quot; &gt; /etc/apt/sources.list.d/ros2-latest.list'</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt update</span></p>

<p class=MsoNormal><span lang=EN-US>$ export ROS_DISTRO=foxy</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt install ros-$ROS_DISTRO-desktop </span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt install
python3-colcon-common-extensions </span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt install python3-rosdep </span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo apt install python3-argcomplete</span></p>

<p class=MsoNormal><span lang=EN-US>$ sudo rosdep init</span></p>

<p class=MsoNormal><span lang=EN-US>$ rosdep update</span></p>

<p class=MsoNormal><span lang=EN-US>$ source /opt/ros/foxy/setup.bash</span></p>

<p class=MsoNormal><span lang=EN-US>$ source ~/.bashrc</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182890"><span style='font-family:"Meiryo UI"'>ワークスペースの作成</span></a><a
href="#_edn1" name="_ednref1" title=""><span class=MsoEndnoteReference><span
lang=EN-US><span class=MsoEndnoteReference><span lang=EN-US style='font-size:
12.0pt;line-height:105%;letter-spacing:.2pt'>[i]</span></span></span></span></a></h3>

<p class=MsoNormal><span lang=EN-US>ROS2</span><span style='font-family:メイリオ'>のインストールが終了したらまず作業領域を作成します。</span></p>

<p class=MsoNormal><span lang=EN-US>$ mkdir -p ~/ros2ws/src</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd ~/ros2ws/src</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182891"><span style='font-family:"Meiryo UI"'>パッケージの作成</span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>続いてパッケージを作成します。ここではパッケージ名を</span><span
lang=EN-US>r2cvr</span><span style='font-family:メイリオ'>などとします。</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd ~/ros2ws/src</span></p>

<p class=MsoNormal><span lang=EN-US>$ ros2 pkg create --build-type ament_python
r2cvr</span></p>

<p class=MsoNormal><span lang=EN-US>$ cd ~/ros2</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>このディレクトリーでビルトします。</span></p>

<p class=MsoNormal><a name="_Hlk75013157"><span lang=EN-US>$ colcon build</span></a></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span><span style='font-family:メイリオ'>以下の行の入力し、パッケージの設定を反映とプログラムを走らせることができます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ . ~/ros2ws/install/setup.bash</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182892"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>ROS</span></a><span style='font-size:16.0pt;
line-height:105%;font-family:"Meiryo UI"'>について</span></h2>

<h3><a name="_Toc80182893"><span style='font-family:"Meiryo UI"'>なぜ<span
lang=EN-US>ROS</span>か<span lang=EN-US>?</span></span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>ロボットはいろいろな仕事をしながらそれぞれが連携して動く必要があります。そのためプログラム間で情報のやり取りを行います。これがプロセス間通信です。マルチタスク化が進み、分担して開発が進めせれるようになってますます</span><span
lang=EN-US>ROS</span><span style='font-family:メイリオ'>の必要性が増してた来ました。さらに高速化、リアルタイム性が求められるようになり、</span><span
lang=EN-US>ROS2</span><span style='font-family:メイリオ'>への移行が進められています。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=535 height=263 id="図 15"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image023.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182894"><span lang=EN-US style='font-family:"Meiryo UI"'>ROS</span></a><span
style='font-family:"Meiryo UI"'>の構造</span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>送りっぱなしの「</span><span
lang=EN-US>Topic</span><span style='font-family:メイリオ'>」と、送ったあと相手から応答を受け取る「</span><span
lang=EN-US>service</span><span style='font-family:メイリオ'>」で通信が行われます。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=525 height=210 id="図 16"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image024.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182895"><span style='font-family:"Meiryo UI"'>分散開発</span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>これによって分散開発が可能となりました。いろいろなプログラミング言語にも対応しています。ここでは</span><span
lang=EN-US>Python3</span><span style='font-family:メイリオ'>使用します。</span></p>

<p class=MsoNormal><span lang=EN-US><img border=0 width=525 height=218 id="図 17"
src="Rros2ComputerVisionお勉強ロボットマニュアルその1_ver1.0.files/image025.png"></span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h2><a name="_Toc80182896"><span lang=EN-US style='font-size:16.0pt;line-height:
105%;font-family:"Meiryo UI"'>ROS2</span></a><span style='font-size:16.0pt;
line-height:105%;font-family:"Meiryo UI"'>を体感する。</span></h2>

<h3><a name="_Toc80182897"><span style='font-family:"Meiryo UI"'>・カメラ画像の取り込み</span></a></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>まずプロジェクトのディレクトリーにある</span><span
lang=EN-US>Setup.py</span><span style='font-family:メイリオ'>の設定をしておきます。</span></p>

<p class=MsoNormal><span lang=EN-US>ubuntu@ubuntu:~/ros2ws/src/r2cvr$</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>この</span><span lang=EN-US>Setup.py</span><span
style='font-family:メイリオ'>に以下のように実行するプログラムを記述しておき、</span><span lang=EN-US>colocon
build</span><span style='font-family:メイリオ'>します。</span></p>

<p class=MsoNormal><span lang=EN-US>entry_points={</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
'console_scripts': [</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
'cam = ' + package_name + '.cam_pub:main',</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
],</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>前述の</span><span lang=EN-US>cam_sample.py</span><span
style='font-family:メイリオ'>を</span><span lang=EN-US>ROS2</span><span
style='font-family:メイリオ'>化ししたものが</span><span lang=EN-US>cam_pub.py</span><span
style='font-family:メイリオ'>で、取り込んだカメラ画像を配信します。カメラを接続して以下を実行してください。</span></p>

<p class=MsoNormal><a name="_Hlk75013721"><span lang=EN-US>$ ros2 run r2cvr cam</span></a></p>

<p class=MsoNormal><span style='font-family:メイリオ'>で画像の</span><span lang=EN-US>Publish</span><span
style='font-family:メイリオ'>します。　</span></p>

<h3><a name="_Toc80182898"><span lang=EN-US style='font-family:"Meiryo UI"'>rqt</span></a><span
style='font-family:"Meiryo UI"'>でカメラ画像を表示します。</span></h3>

<p class=MsoNormal><span style='font-family:メイリオ'>新しいターミナルで</span><span
lang=EN-US>rqt</span><span style='font-family:メイリオ'>を立ち上げます。</span></p>

<p class=MsoNormal><span lang=EN-US>$ rqt</span></p>

<p class=MsoNormal><span lang=EN-US>Plugin</span><span style='font-family:メイリオ'>の</span><span
lang=EN-US>Visualization</span><span style='font-family:メイリオ'>から</span><span
lang=EN-US>Image view</span><span style='font-family:メイリオ'>を選択し、</span><span
lang=EN-US>/img_topic</span><span style='font-family:メイリオ'>を表示します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>カメラ画像を見ることができます。もう一台</span><span
lang=EN-US>PC</span><span style='font-family:メイリオ'>があれば</span><span lang=EN-US>ROS2</span><span
style='font-family:メイリオ'>を同じネットワーク上で走らせておくと同様に表示できます。</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

<h3><a name="_Toc80182899"><span lang=EN-US style='font-family:"Meiryo UI"'>rosbag2</span></a><span
style='font-family:"Meiryo UI"'>で録画してみよう。</span></h3>

<p class=MsoNormal><span lang=EN-US>$ ros2 bag record -o all.bag -a</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>ですべての</span><span lang=EN-US>Topic</span><span
style='font-family:メイリオ'>を</span><span lang=EN-US>all.bag</span><span
style='font-family:メイリオ'>に保存します。</span><span lang=EN-US>Ctl-C</span><span
style='font-family:メイリオ'>で終了します。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>再生は以下です。配信プログラムを停止し、以下を実行します。</span></p>

<p class=MsoNormal><span lang=EN-US>$ ros2 bag play all.bag</span></p>

<p class=MsoNormal><span lang=EN-US>Rqt</span><span style='font-family:メイリオ'>で保存した画像を確認することができます。</span></p>

<p class=MsoNormal><span style='font-family:メイリオ'>個々の</span><span lang=EN-US>Topic</span><span
style='font-family:メイリオ'>を保存する場合は以下です。この例では</span><span lang=EN-US>img_topic</span><span
style='font-family:メイリオ'>を</span><span lang=EN-US>topic.bag</span><span
style='font-family:メイリオ'>に保存します。</span></p>

<p class=MsoNormal><span lang=EN-US>$ ros2 bag record -o <a name="_Hlk75012379">topic.bag</a>
/img_topic</span></p>

<p class=MsoNormal><span lang=EN-US>&nbsp;</span></p>

</div>

<div><br clear=all>

<hr align=left size=1 width="33%">

<div id=edn1>

<p class=MsoEndnoteText><a href="#_ednref1" name="_edn1" title=""></a><span
lang=EN-US>&nbsp;</span></p>

</div>

</div>

</body>

</html>
