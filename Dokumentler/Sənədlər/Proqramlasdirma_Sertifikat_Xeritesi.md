<!DOCTYPE html>

<html lang="az">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Proqramlaşdırma Dalları və Sertifikatları</title>

<style>

&#x20; @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700\&display=swap');



&#x20; \* { margin: 0; padding: 0; box-sizing: border-box; }



&#x20; body {

&#x20;   font-family: 'Inter', sans-serif;

&#x20;   background: #fff;

&#x20;   color: #1a1a1a;

&#x20;   padding: 40px 30px;

&#x20; }



&#x20; h1.page-title {

&#x20;   text-align: center;

&#x20;   font-size: 2rem;

&#x20;   font-weight: 700;

&#x20;   margin-bottom: 8px;

&#x20;   border-bottom: 2px solid #1a1a1a;

&#x20;   padding-bottom: 12px;

&#x20; }



&#x20; h2.section-title {

&#x20;   font-size: 1.4rem;

&#x20;   font-weight: 700;

&#x20;   margin: 30px 0 16px;

&#x20; }



&#x20; /\* ======= MAIN GRID ======= \*/

&#x20; .grid-container {

&#x20;   width: 100%;

&#x20;   overflow-x: auto;

&#x20; }



&#x20; table.cert-table {

&#x20;   border-collapse: collapse;

&#x20;   width: 100%;

&#x20;   min-width: 1100px;

&#x20;   font-size: 10.5px;

&#x20; }



&#x20; /\* Column headers \*/

&#x20; .col-header {

&#x20;   text-align: center;

&#x20;   font-size: 10px;

&#x20;   font-weight: 700;

&#x20;   padding: 6px 4px;

&#x20;   border: 1px solid #ccc;

&#x20;   background: #f0f0f0;

&#x20;   vertical-align: bottom;

&#x20; }



&#x20; .col-header.highlight-blue { background: #d6e8f7; color: #0056b3; }

&#x20; .col-header.highlight-orange { background: #fde8cc; color: #b35c00; }

&#x20; .col-header.highlight-green { background: #d9f0d5; color: #2e6e25; }

&#x20; .col-header.highlight-purple { background: #ecddf7; color: #5e1a8c; }

&#x20; .col-header.highlight-red { background: #fdd9d9; color: #8c0000; }

&#x20; .col-header.highlight-teal { background: #d0f0ee; color: #0a5c58; }



&#x20; /\* Level labels \*/

&#x20; .level-cell {

&#x20;   font-size: 10px;

&#x20;   font-weight: 700;

&#x20;   writing-mode: vertical-lr;

&#x20;   transform: rotate(180deg);

&#x20;   text-align: center;

&#x20;   padding: 6px 4px;

&#x20;   background: #f5f5f5;

&#x20;   border: 1px solid #ccc;

&#x20;   white-space: nowrap;

&#x20;   color: #333;

&#x20; }



&#x20; /\* Cert boxes \*/

&#x20; td.cert-cell {

&#x20;   border: 1px solid #ddd;

&#x20;   padding: 3px;

&#x20;   vertical-align: top;

&#x20;   min-width: 80px;

&#x20; }



&#x20; .cert-box {

&#x20;   display: inline-block;

&#x20;   font-size: 9.5px;

&#x20;   font-weight: 600;

&#x20;   padding: 3px 5px;

&#x20;   border-radius: 3px;

&#x20;   margin: 2px;

&#x20;   cursor: default;

&#x20;   line-height: 1.3;

&#x20;   text-align: center;

&#x20;   white-space: nowrap;

&#x20; }



&#x20; /\* Color themes for cert boxes \*/

&#x20; .c-blue    { background: #d6e8f7; color: #003f7f; border: 1px solid #a8cce8; }

&#x20; .c-orange  { background: #fde8cc; color: #7a3c00; border: 1px solid #f0c070; }

&#x20; .c-green   { background: #d9f0d5; color: #1e5218; border: 1px solid #9fd494; }

&#x20; .c-purple  { background: #ecddf7; color: #4a0f78; border: 1px solid #c9a0e8; }

&#x20; .c-red     { background: #fdd9d9; color: #6e0000; border: 1px solid #f5a0a0; }

&#x20; .c-teal    { background: #d0f0ee; color: #0a3e3c; border: 1px solid #80ccc9; }

&#x20; .c-gray    { background: #ebebeb; color: #2a2a2a; border: 1px solid #bbb; }

&#x20; .c-yellow  { background: #fffacc; color: #5a4500; border: 1px solid #e8d86a; }

&#x20; .c-brown   { background: #f2e5d5; color: #4a2800; border: 1px solid #c8a070; }

&#x20; .c-pink    { background: #fde0ee; color: #6e0040; border: 1px solid #f0a0cc; }



&#x20; /\* group header spanning row \*/

&#x20; td.group-header {

&#x20;   background: #2a2a2a;

&#x20;   color: #fff;

&#x20;   font-size: 11px;

&#x20;   font-weight: 700;

&#x20;   text-align: center;

&#x20;   padding: 5px;

&#x20;   letter-spacing: 0.5px;

&#x20; }



&#x20; /\* Sub-category label row \*/

&#x20; td.sub-header {

&#x20;   background: #e8e8e8;

&#x20;   font-size: 9.5px;

&#x20;   font-weight: 600;

&#x20;   text-align: center;

&#x20;   padding: 3px;

&#x20;   color: #333;

&#x20;   border: 1px solid #ccc;

&#x20;   font-style: italic;

&#x20; }



&#x20; /\* empty cell \*/

&#x20; td.empty-cell {

&#x20;   border: 1px solid #eee;

&#x20;   background: #fafafa;

&#x20; }



&#x20; /\* ======= LEGEND ======= \*/

&#x20; .legend {

&#x20;   margin-top: 20px;

&#x20;   display: flex;

&#x20;   flex-wrap: wrap;

&#x20;   gap: 10px;

&#x20;   font-size: 11px;

&#x20; }

&#x20; .legend-item {

&#x20;   display: flex;

&#x20;   align-items: center;

&#x20;   gap: 6px;

&#x20; }

&#x20; .legend-box {

&#x20;   width: 24px; height: 14px;

&#x20;   border-radius: 2px;

&#x20; }



&#x20; /\* ======= DETAIL SECTION ======= \*/

&#x20; .detail-section {

&#x20;   margin-top: 40px;

&#x20; }



&#x20; .detail-section h3 {

&#x20;   font-size: 1rem;

&#x20;   font-weight: 700;

&#x20;   color: #1a4f8a;

&#x20;   border-left: 4px solid #1a4f8a;

&#x20;   padding-left: 10px;

&#x20;   margin: 20px 0 8px;

&#x20; }



&#x20; .detail-section p {

&#x20;   font-size: 12px;

&#x20;   color: #444;

&#x20;   line-height: 1.6;

&#x20;   max-width: 900px;

&#x20; }



&#x20; .note {

&#x20;   font-size: 11px;

&#x20;   color: #555;

&#x20;   margin-top: 14px;

&#x20;   font-style: italic;

&#x20; }



&#x20; .count-note {

&#x20;   text-align: right;

&#x20;   font-size: 11px;

&#x20;   color: #666;

&#x20;   margin-top: 8px;

&#x20; }

</style>

</head>

<body>



<h1 class="page-title">Proqramlaşdırma</h1>

<h2 class="section-title">Proqramlaşdırma Dalları və Sertifikatları</h2>



<div class="grid-container">

<table class="cert-table">

&#x20; <thead>

&#x20;   <tr>

&#x20;     <td style="border:none;" colspan="2"></td>

&#x20;     <th class="col-header highlight-blue" colspan="2">Veb İnkişafı<br><small>(Web Dev)</small></th>

&#x20;     <th class="col-header highlight-orange" colspan="3">Bulud Hesablama<br><small>(Cloud)</small></th>

&#x20;     <th class="col-header highlight-purple" colspan="2">Proqramlaşdırma<br>Dilləri</th>

&#x20;     <th class="col-header highlight-green" colspan="2">Verilənlər Bazası<br><small>(Database)</small></th>

&#x20;     <th class="col-header highlight-red" colspan="2">DevOps /<br>Konteyner</th>

&#x20;     <th class="col-header highlight-teal" colspan="2">Mobil / Digər</th>

&#x20;   </tr>

&#x20;   <tr>

&#x20;     <td style="border:none;" colspan="2"></td>

&#x20;     <th class="col-header" style="background:#e8f0fb">Frontend</th>

&#x20;     <th class="col-header" style="background:#e8f0fb">Backend /<br>Full-Stack</th>

&#x20;     <th class="col-header" style="background:#fef0dc">AWS</th>

&#x20;     <th class="col-header" style="background:#fef0dc">Azure /<br>Microsoft</th>

&#x20;     <th class="col-header" style="background:#fef0dc">Google Cloud</th>

&#x20;     <th class="col-header" style="background:#f0e8fb">Java</th>

&#x20;     <th class="col-header" style="background:#f0e8fb">Python /<br>Digər</th>

&#x20;     <th class="col-header" style="background:#e8f7e8">SQL / Oracle</th>

&#x20;     <th class="col-header" style="background:#e8f7e8">NoSQL /<br>MongoDB</th>

&#x20;     <th class="col-header" style="background:#fde8e8">Docker /<br>Kubernetes</th>

&#x20;     <th class="col-header" style="background:#fde8e8">CI/CD /<br>Agile</th>

&#x20;     <th class="col-header" style="background:#e0f7f5">Android /<br>iOS</th>

&#x20;     <th class="col-header" style="background:#e0f7f5">Digər /<br>Crossplatform</th>

&#x20;   </tr>

&#x20; </thead>

&#x20; <tbody>



&#x20;   <!-- EXPERT ROW -->

&#x20;   <tr>

&#x20;     <td class="level-cell" rowspan="4">Ekspert</td>

&#x20;     <td class="cert-cell" style="background:#f9f9f9; font-size:9px; font-weight:700; color:#666; text-align:center; width:60px;">Mütəxəssis</td>

&#x20;     <!-- Frontend -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">W3C Dev Cert</span>

&#x20;     </td>

&#x20;     <!-- Full-Stack -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">IBM Full Stack Adv</span>

&#x20;       <span class="cert-box c-blue">JSNAD</span>

&#x20;       <span class="cert-box c-blue">JSNSD</span>

&#x20;     </td>

&#x20;     <!-- AWS -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AWS SA Pro</span>

&#x20;       <span class="cert-box c-orange">AWS DevOps Pro</span>

&#x20;       <span class="cert-box c-orange">AWS ML Specialty</span>

&#x20;     </td>

&#x20;     <!-- Azure -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AZ-305 SA Expert</span>

&#x20;       <span class="cert-box c-orange">AZ-400 DevOps</span>

&#x20;     </td>

&#x20;     <!-- GCP -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">GCP Prof Cloud Dev</span>

&#x20;       <span class="cert-box c-orange">GCP Data Engineer</span>

&#x20;     </td>

&#x20;     <!-- Java -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">OCP Java SE 17</span>

&#x20;       <span class="cert-box c-purple">Red Hat EX183</span>

&#x20;       <span class="cert-box c-purple">Spring Pro</span>

&#x20;     </td>

&#x20;     <!-- Python -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">PCPP (Python Inst)</span>

&#x20;       <span class="cert-box c-purple">TensorFlow Dev</span>

&#x20;       <span class="cert-box c-purple">IEEE CSDP</span>

&#x20;     </td>

&#x20;     <!-- SQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">Oracle DB Admin</span>

&#x20;       <span class="cert-box c-green">MS SQL Expert</span>

&#x20;     </td>

&#x20;     <!-- NoSQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">Elastic Certified Eng</span>

&#x20;       <span class="cert-box c-green">Redis Certified</span>

&#x20;     </td>

&#x20;     <!-- DevOps -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">CKA</span>

&#x20;       <span class="cert-box c-red">CKAD</span>

&#x20;       <span class="cert-box c-red">CKS</span>

&#x20;     </td>

&#x20;     <!-- Agile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">PMP</span>

&#x20;       <span class="cert-box c-red">SAFe Agilist</span>

&#x20;       <span class="cert-box c-red">CSD</span>

&#x20;     </td>

&#x20;     <!-- Mobile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Google Android Assoc</span>

&#x20;     </td>

&#x20;     <!-- Cross -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Salesforce Dev I</span>

&#x20;       <span class="cert-box c-teal">HashiCorp Terraform</span>

&#x20;     </td>

&#x20;   </tr>



&#x20;   <tr>

&#x20;     <td class="cert-cell" style="background:#f9f9f9; font-size:9px; font-weight:700; color:#666; text-align:center; width:60px;"></td>

&#x20;     <!-- Frontend -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">Meta Front-End Pro</span>

&#x20;     </td>

&#x20;     <!-- Full-Stack -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">OpenJS Fdn Cert</span>

&#x20;     </td>

&#x20;     <!-- AWS -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AWS SA Associate</span>

&#x20;     </td>

&#x20;     <!-- Azure -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AZ-204 Dev Assoc</span>

&#x20;     </td>

&#x20;     <!-- GCP -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">GCP Assoc Cloud Eng</span>

&#x20;     </td>

&#x20;     <!-- Java -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">PCAP (Python Inst)</span>

&#x20;     </td>

&#x20;     <!-- Python -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">Databricks Spark</span>

&#x20;     </td>

&#x20;     <!-- SQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">Oracle SQL Pro</span>

&#x20;     </td>

&#x20;     <!-- NoSQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">MongoDB Certified Dev</span>

&#x20;     </td>

&#x20;     <!-- DevOps -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">Docker DCA</span>

&#x20;     </td>

&#x20;     <!-- Agile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">CSM</span>

&#x20;       <span class="cert-box c-red">PMI-ACP</span>

&#x20;     </td>

&#x20;     <!-- Mobile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Apple Cert iOS Dev</span>

&#x20;     </td>

&#x20;     <!-- Cross -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Apache Kafka CCDAK</span>

&#x20;     </td>

&#x20;   </tr>



&#x20;   <!-- INTERMEDIATE ROW -->

&#x20;   <tr>

&#x20;     <td class="level-cell" rowspan="3" style="background:#f0f0f0; writing-mode:vertical-lr; transform:rotate(180deg);">Orta</td>

&#x20;     <td class="cert-cell" style="background:#f9f9f9; font-size:9px; font-weight:700; color:#666; text-align:center;"></td>

&#x20;     <!-- Frontend -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">Meta Front-End Dev</span>

&#x20;       <span class="cert-box c-blue">fCC Responsive Web</span>

&#x20;     </td>

&#x20;     <!-- Full-Stack -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">IBM Full Stack Dev</span>

&#x20;       <span class="cert-box c-blue">fCC JS Algo</span>

&#x20;     </td>

&#x20;     <!-- AWS -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AWS Developer Assoc</span>

&#x20;       <span class="cert-box c-orange">AWS SysOps</span>

&#x20;     </td>

&#x20;     <!-- Azure -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AZ-104 Admin</span>

&#x20;       <span class="cert-box c-orange">AZ-900 Fdn</span>

&#x20;     </td>

&#x20;     <!-- GCP -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">Google IT Automation</span>

&#x20;     </td>

&#x20;     <!-- Java -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">OCA Java SE 8</span>

&#x20;       <span class="cert-box c-purple">1Z0-808</span>

&#x20;     </td>

&#x20;     <!-- Python -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">PCEP (Python Inst)</span>

&#x20;       <span class="cert-box c-purple">MS Python Dev</span>

&#x20;     </td>

&#x20;     <!-- SQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">Oracle SQL Assoc</span>

&#x20;       <span class="cert-box c-green">1Z0-071</span>

&#x20;     </td>

&#x20;     <!-- NoSQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">MongoDB Python Dev</span>

&#x20;     </td>

&#x20;     <!-- DevOps -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">Linux Foundation CKA</span>

&#x20;     </td>

&#x20;     <!-- Agile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">PSM I</span>

&#x20;       <span class="cert-box c-red">CAPM</span>

&#x20;     </td>

&#x20;     <!-- Mobile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Meta Android Dev</span>

&#x20;     </td>

&#x20;     <!-- Cross -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Salesforce Admin</span>

&#x20;     </td>

&#x20;   </tr>



&#x20;   <tr>

&#x20;     <td class="cert-cell" style="background:#f9f9f9; font-size:9px; color:#666; text-align:center;"></td>

&#x20;     <!-- Frontend -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">fCC Front End Libs</span>

&#x20;     </td>

&#x20;     <!-- Full-Stack -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-blue">The Odin Project</span>

&#x20;     </td>

&#x20;     <!-- AWS -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">AWS Cloud Practitioner</span>

&#x20;     </td>

&#x20;     <!-- Azure -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">PL-900 Power Platform</span>

&#x20;     </td>

&#x20;     <!-- GCP -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-orange">Oracle OCI Fdn</span>

&#x20;     </td>

&#x20;     <!-- Java -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">Zend PHP Dev</span>

&#x20;     </td>

&#x20;     <!-- Python -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-purple">DataCamp Data Sci</span>

&#x20;     </td>

&#x20;     <!-- SQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">MS Certified: Data</span>

&#x20;     </td>

&#x20;     <!-- NoSQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-green">Cassandra Dev</span>

&#x20;     </td>

&#x20;     <!-- DevOps -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">GitLab CI/CD Cert</span>

&#x20;     </td>

&#x20;     <!-- Agile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-red">Scrum.org PSM</span>

&#x20;     </td>

&#x20;     <!-- Mobile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">Flutter Dev Cert</span>

&#x20;     </td>

&#x20;     <!-- Cross -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-teal">HackerRank Skills</span>

&#x20;     </td>

&#x20;   </tr>



&#x20;   <!-- BEGINNER ROW -->

&#x20;   <tr>

&#x20;     <td class="level-cell" style="background:#e8e8e8; writing-mode:vertical-lr; transform:rotate(180deg);">Başlanğıc</td>

&#x20;     <td class="cert-cell" style="background:#f9f9f9; font-size:9px; color:#666; text-align:center;"></td>

&#x20;     <!-- Frontend -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">fCC Responsive Web</span>

&#x20;       <span class="cert-box c-gray">HTML/CSS Cert</span>

&#x20;     </td>

&#x20;     <!-- Full-Stack -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">IBM Full Stack (Coursera)</span>

&#x20;       <span class="cert-box c-gray">CS50x Harvard</span>

&#x20;     </td>

&#x20;     <!-- AWS -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-yellow">AWS Cloud Practitioner</span>

&#x20;       <span class="cert-box c-yellow">CLF-C02</span>

&#x20;     </td>

&#x20;     <!-- Azure -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-yellow">AZ-900</span>

&#x20;       <span class="cert-box c-yellow">MS Fundamentals</span>

&#x20;     </td>

&#x20;     <!-- GCP -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-yellow">Google Workspace Cert</span>

&#x20;     </td>

&#x20;     <!-- Java -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">Codecademy Java</span>

&#x20;       <span class="cert-box c-gray">MOOC.fi Java</span>

&#x20;     </td>

&#x20;     <!-- Python -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">Google IT Auto Python</span>

&#x20;       <span class="cert-box c-gray">Kaggle Python</span>

&#x20;     </td>

&#x20;     <!-- SQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">fCC Relational DB</span>

&#x20;       <span class="cert-box c-gray">SQLZoo Cert</span>

&#x20;     </td>

&#x20;     <!-- NoSQL -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">MongoDB Basics</span>

&#x20;     </td>

&#x20;     <!-- DevOps -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">Git / GitHub Cert</span>

&#x20;     </td>

&#x20;     <!-- Agile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">Scrum Intro</span>

&#x20;       <span class="cert-box c-gray">Kanban Fdn</span>

&#x20;     </td>

&#x20;     <!-- Mobile -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">Codecademy Mobile</span>

&#x20;     </td>

&#x20;     <!-- Cross -->

&#x20;     <td class="cert-cell">

&#x20;       <span class="cert-box c-gray">Pccet (CompTIA)</span>

&#x20;     </td>

&#x20;   </tr>



&#x20; </tbody>

</table>

</div>



<p class="count-note">70+ sertifikat sıralanmışdır | Fevral 2026</p>



<p class="note">\* Yuxarıda günümüzdə yaygın olaraq yer alan proqramlaşdırma dalları və bu dallarda etkin istifadə olunan sertifikatları görə bilərsiniz.</p>



<!-- ============ DETAIL SECTION ============ -->

<div class="detail-section">



&#x20; <h3>Veb İnkişafı (Web Development)</h3>

&#x20; <p>

&#x20;   Frontend, Backend və Full-Stack sahələrini əhatə edir. HTML, CSS, JavaScript əsasları ilə başlayaraq React, Node.js, Django kimi freymvorklara qədər uzanır.

&#x20;   <strong>freeCodeCamp</strong> sertifikatları tamamilə pulsuzdur. <strong>Meta Professional Certificates</strong> işəgötürənlər tərəfindən tanınan sertifikatlardır.

&#x20;   Backend proqramçılar üçün <strong>JSNAD / JSNSD</strong> (Linux Foundation) Node.js üzrə ən tanınan rəsmi sertifikatlardır.

&#x20; </p>



&#x20; <h3>Bulud Hesablama (Cloud Computing)</h3>

&#x20; <p>

&#x20;   AWS, Microsoft Azure və Google Cloud üzrə sertifikatlar proqramçılar üçün ən yüksək maaş artımını təmin edən sertifikat qrupudur.

&#x20;   Başlanğıc üçün: <strong>AWS Cloud Practitioner (CLF-C02)</strong> ($100) və ya <strong>AZ-900 Azure Fundamentals</strong> (\~$165) tövsiyə olunur.

&#x20;   Orta səviyyə: <strong>AWS Developer Associate (DVA-C02)</strong> ($150). Ekspert: <strong>AWS Solutions Architect Professional</strong> ($300).

&#x20; </p>



&#x20; <h3>Java Proqramlaşdırması</h3>

&#x20; <p>

&#x20;   Oracle tərəfindən verilən <strong>OCA Java SE 8 (1Z0-808)</strong> → <strong>OCP Java SE 17 (1Z0-829)</strong> yolu ən klassik Java sertifikat yoludur.

&#x20;   Enterprise tərəf üçün <strong>Red Hat EX183</strong> əlavə edilə bilər. Java proqramçılarının qlobal ortalama maaşı \~$95,000-$150,000/il arasındadır.

&#x20; </p>



&#x20; <h3>Python / Data Science / AI</h3>

&#x20; <p>

&#x20;   Python Institute-un <strong>PCEP → PCAP → PCPP</strong> sertifikat pilləsi tam strukturlu bir yol təklif edir.

&#x20;   Data Science sahəsinə keçmək istəyənlər üçün <strong>Google IT Automation with Python</strong> (Coursera, \~$49/ay) ideal başlanğıc nöqtəsidir.

&#x20;   AI/ML üçün isə <strong>TensorFlow Developer Certification</strong> ($100) və <strong>AWS ML Specialty</strong> ($300) tövsiyə olunur.

&#x20; </p>



&#x20; <h3>DevOps / Konteyner</h3>

&#x20; <p>

&#x20;   <strong>Docker Certified Associate (DCA)</strong> ($400) → <strong>CKAD</strong> ($395) → <strong>CKA</strong> ($395) sırası DevOps karyerası üçün standart yoldur.

&#x20;   Daha mürəkkəb mühitlər üçün <strong>CKS (Certified Kubernetes Security Specialist)</strong> əlavə edilə bilər.

&#x20;   CI/CD sahəsində <strong>GitLab CI/CD Certification</strong> praktiki mənada çox dəyərlidir.

&#x20; </p>



&#x20; <h3>Verilənlər Bazası (Database)</h3>

&#x20; <p>

&#x20;   SQL tərəf üçün <strong>Oracle SQL Certified Associate (1Z0-071)</strong> (\~$245) ən populyar sertifikatlardandır.

&#x20;   NoSQL tərəf üçün <strong>MongoDB Certified Developer Associate</strong> ($150) öndə gəlir.

&#x20;   Böyük məlumat (Big Data) sahəsi üçün <strong>Databricks Apache Spark</strong> sertifikatı qiymətlidir.

&#x20; </p>



</div>



</body>

</html>

