<!DOCTYPE html>
<html lang="az">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Proqramlaşdırma Dalları və Sertifikatları</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Inter', sans-serif;
    background: #fff;
    color: #1a1a1a;
    padding: 40px 30px;
  }

  h1.page-title {
    text-align: center;
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 8px;
    border-bottom: 2px solid #1a1a1a;
    padding-bottom: 12px;
  }

  h2.section-title {
    font-size: 1.4rem;
    font-weight: 700;
    margin: 30px 0 16px;
  }

  /* ======= MAIN GRID ======= */
  .grid-container {
    width: 100%;
    overflow-x: auto;
  }

  table.cert-table {
    border-collapse: collapse;
    width: 100%;
    min-width: 1100px;
    font-size: 10.5px;
  }

  /* Column headers */
  .col-header {
    text-align: center;
    font-size: 10px;
    font-weight: 700;
    padding: 6px 4px;
    border: 1px solid #ccc;
    background: #f0f0f0;
    vertical-align: bottom;
  }

  .col-header.highlight-blue { background: #d6e8f7; color: #0056b3; }
  .col-header.highlight-orange { background: #fde8cc; color: #b35c00; }
  .col-header.highlight-green { background: #d9f0d5; color: #2e6e25; }
  .col-header.highlight-purple { background: #ecddf7; color: #5e1a8c; }
  .col-header.highlight-red { background: #fdd9d9; color: #8c0000; }
  .col-header.highlight-teal { background: #d0f0ee; color: #0a5c58; }

  /* Level labels */
  .level-cell {
    font-size: 10px;
    font-weight: 700;
    writing-mode: vertical-lr;
    transform: rotate(180deg);
    text-align: center;
    padding: 6px 4px;
    background: #f5f5f5;
    border: 1px solid #ccc;
    white-space: nowrap;
    color: #333;
  }

  /* Cert boxes */
  td.cert-cell {
    border: 1px solid #ddd;
    padding: 3px;
    vertical-align: top;
    min-width: 80px;
  }

  .cert-box {
    display: inline-block;
    font-size: 9.5px;
    font-weight: 600;
    padding: 3px 5px;
    border-radius: 3px;
    margin: 2px;
    cursor: default;
    line-height: 1.3;
    text-align: center;
    white-space: nowrap;
  }

  /* Color themes for cert boxes */
  .c-blue    { background: #d6e8f7; color: #003f7f; border: 1px solid #a8cce8; }
  .c-orange  { background: #fde8cc; color: #7a3c00; border: 1px solid #f0c070; }
  .c-green   { background: #d9f0d5; color: #1e5218; border: 1px solid #9fd494; }
  .c-purple  { background: #ecddf7; color: #4a0f78; border: 1px solid #c9a0e8; }
  .c-red     { background: #fdd9d9; color: #6e0000; border: 1px solid #f5a0a0; }
  .c-teal    { background: #d0f0ee; color: #0a3e3c; border: 1px solid #80ccc9; }
  .c-gray    { background: #ebebeb; color: #2a2a2a; border: 1px solid #bbb; }
  .c-yellow  { background: #fffacc; color: #5a4500; border: 1px solid #e8d86a; }
  .c-brown   { background: #f2e5d5; color: #4a2800; border: 1px solid #c8a070; }
  .c-pink    { background: #fde0ee; color: #6e0040; border: 1px solid #f0a0cc; }

  /* group header spanning row */
  td.group-header {
    background: #2a2a2a;
    color: #fff;
    font-size: 11px;
    font-weight: 700;
    text-align: center;
    padding: 5px;
    letter-spacing: 0.5px;
  }

  /* Sub-category label row */
  td.sub-header {
    background: #e8e8e8;
    font-size: 9.5px;
    font-weight: 600;
    text-align: center;
    padding: 3px;
    color: #333;
    border: 1px solid #ccc;
    font-style: italic;
  }

  /* empty cell */
  td.empty-cell {
    border: 1px solid #eee;
    background: #fafafa;
  }

  /* ======= LEGEND ======= */
  .legend {
    margin-top: 20px;
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    font-size: 11px;
  }
  .legend-item {
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .legend-box {
    width: 24px; height: 14px;
    border-radius: 2px;
  }

  /* ======= DETAIL SECTION ======= */
  .detail-section {
    margin-top: 40px;
  }

  .detail-section h3 {
    font-size: 1rem;
    font-weight: 700;
    color: #1a4f8a;
    border-left: 4px solid #1a4f8a;
    padding-left: 10px;
    margin: 20px 0 8px;
  }

  .detail-section p {
    font-size: 12px;
    color: #444;
    line-height: 1.6;
    max-width: 900px;
  }

  .note {
    font-size: 11px;
    color: #555;
    margin-top: 14px;
    font-style: italic;
  }

  .count-note {
    text-align: right;
    font-size: 11px;
    color: #666;
    margin-top: 8px;
  }
</style>
</head>
<body>

<h1 class="page-title">Proqramlaşdırma</h1>
<h2 class="section-title">Proqramlaşdırma Dalları və Sertifikatları</h2>

<div class="grid-container">
<table class="cert-table">
  <thead>
    <tr>
      <td style="border:none;" colspan="2"></td>
      <th class="col-header highlight-blue" colspan="2">Veb İnkişafı<br><small>(Web Dev)</small></th>
      <th class="col-header highlight-orange" colspan="3">Bulud Hesablama<br><small>(Cloud)</small></th>
      <th class="col-header highlight-purple" colspan="2">Proqramlaşdırma<br>Dilləri</th>
      <th class="col-header highlight-green" colspan="2">Verilənlər Bazası<br><small>(Database)</small></th>
      <th class="col-header highlight-red" colspan="2">DevOps /<br>Konteyner</th>
      <th class="col-header highlight-teal" colspan="2">Mobil / Digər</th>
    </tr>
    <tr>
      <td style="border:none;" colspan="2"></td>
      <th class="col-header" style="background:#e8f0fb">Frontend</th>
      <th class="col-header" style="background:#e8f0fb">Backend /<br>Full-Stack</th>
      <th class="col-header" style="background:#fef0dc">AWS</th>
      <th class="col-header" style="background:#fef0dc">Azure /<br>Microsoft</th>
      <th class="col-header" style="background:#fef0dc">Google Cloud</th>
      <th class="col-header" style="background:#f0e8fb">Java</th>
      <th class="col-header" style="background:#f0e8fb">Python /<br>Digər</th>
      <th class="col-header" style="background:#e8f7e8">SQL / Oracle</th>
      <th class="col-header" style="background:#e8f7e8">NoSQL /<br>MongoDB</th>
      <th class="col-header" style="background:#fde8e8">Docker /<br>Kubernetes</th>
      <th class="col-header" style="background:#fde8e8">CI/CD /<br>Agile</th>
      <th class="col-header" style="background:#e0f7f5">Android /<br>iOS</th>
      <th class="col-header" style="background:#e0f7f5">Digər /<br>Crossplatform</th>
    </tr>
  </thead>
  <tbody>

    <!-- EXPERT ROW -->
    <tr>
      <td class="level-cell" rowspan="4">Ekspert</td>
      <td class="cert-cell" style="background:#f9f9f9; font-size:9px; font-weight:700; color:#666; text-align:center; width:60px;">Mütəxəssis</td>
      <!-- Frontend -->
      <td class="cert-cell">
        <span class="cert-box c-blue">W3C Dev Cert</span>
      </td>
      <!-- Full-Stack -->
      <td class="cert-cell">
        <span class="cert-box c-blue">IBM Full Stack Adv</span>
        <span class="cert-box c-blue">JSNAD</span>
        <span class="cert-box c-blue">JSNSD</span>
      </td>
      <!-- AWS -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AWS SA Pro</span>
        <span class="cert-box c-orange">AWS DevOps Pro</span>
        <span class="cert-box c-orange">AWS ML Specialty</span>
      </td>
      <!-- Azure -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AZ-305 SA Expert</span>
        <span class="cert-box c-orange">AZ-400 DevOps</span>
      </td>
      <!-- GCP -->
      <td class="cert-cell">
        <span class="cert-box c-orange">GCP Prof Cloud Dev</span>
        <span class="cert-box c-orange">GCP Data Engineer</span>
      </td>
      <!-- Java -->
      <td class="cert-cell">
        <span class="cert-box c-purple">OCP Java SE 17</span>
        <span class="cert-box c-purple">Red Hat EX183</span>
        <span class="cert-box c-purple">Spring Pro</span>
      </td>
      <!-- Python -->
      <td class="cert-cell">
        <span class="cert-box c-purple">PCPP (Python Inst)</span>
        <span class="cert-box c-purple">TensorFlow Dev</span>
        <span class="cert-box c-purple">IEEE CSDP</span>
      </td>
      <!-- SQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">Oracle DB Admin</span>
        <span class="cert-box c-green">MS SQL Expert</span>
      </td>
      <!-- NoSQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">Elastic Certified Eng</span>
        <span class="cert-box c-green">Redis Certified</span>
      </td>
      <!-- DevOps -->
      <td class="cert-cell">
        <span class="cert-box c-red">CKA</span>
        <span class="cert-box c-red">CKAD</span>
        <span class="cert-box c-red">CKS</span>
      </td>
      <!-- Agile -->
      <td class="cert-cell">
        <span class="cert-box c-red">PMP</span>
        <span class="cert-box c-red">SAFe Agilist</span>
        <span class="cert-box c-red">CSD</span>
      </td>
      <!-- Mobile -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Google Android Assoc</span>
      </td>
      <!-- Cross -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Salesforce Dev I</span>
        <span class="cert-box c-teal">HashiCorp Terraform</span>
      </td>
    </tr>

    <tr>
      <td class="cert-cell" style="background:#f9f9f9; font-size:9px; font-weight:700; color:#666; text-align:center; width:60px;"></td>
      <!-- Frontend -->
      <td class="cert-cell">
        <span class="cert-box c-blue">Meta Front-End Pro</span>
      </td>
      <!-- Full-Stack -->
      <td class="cert-cell">
        <span class="cert-box c-blue">OpenJS Fdn Cert</span>
      </td>
      <!-- AWS -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AWS SA Associate</span>
      </td>
      <!-- Azure -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AZ-204 Dev Assoc</span>
      </td>
      <!-- GCP -->
      <td class="cert-cell">
        <span class="cert-box c-orange">GCP Assoc Cloud Eng</span>
      </td>
      <!-- Java -->
      <td class="cert-cell">
        <span class="cert-box c-purple">PCAP (Python Inst)</span>
      </td>
      <!-- Python -->
      <td class="cert-cell">
        <span class="cert-box c-purple">Databricks Spark</span>
      </td>
      <!-- SQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">Oracle SQL Pro</span>
      </td>
      <!-- NoSQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">MongoDB Certified Dev</span>
      </td>
      <!-- DevOps -->
      <td class="cert-cell">
        <span class="cert-box c-red">Docker DCA</span>
      </td>
      <!-- Agile -->
      <td class="cert-cell">
        <span class="cert-box c-red">CSM</span>
        <span class="cert-box c-red">PMI-ACP</span>
      </td>
      <!-- Mobile -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Apple Cert iOS Dev</span>
      </td>
      <!-- Cross -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Apache Kafka CCDAK</span>
      </td>
    </tr>

    <!-- INTERMEDIATE ROW -->
    <tr>
      <td class="level-cell" rowspan="3" style="background:#f0f0f0; writing-mode:vertical-lr; transform:rotate(180deg);">Orta</td>
      <td class="cert-cell" style="background:#f9f9f9; font-size:9px; font-weight:700; color:#666; text-align:center;"></td>
      <!-- Frontend -->
      <td class="cert-cell">
        <span class="cert-box c-blue">Meta Front-End Dev</span>
        <span class="cert-box c-blue">fCC Responsive Web</span>
      </td>
      <!-- Full-Stack -->
      <td class="cert-cell">
        <span class="cert-box c-blue">IBM Full Stack Dev</span>
        <span class="cert-box c-blue">fCC JS Algo</span>
      </td>
      <!-- AWS -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AWS Developer Assoc</span>
        <span class="cert-box c-orange">AWS SysOps</span>
      </td>
      <!-- Azure -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AZ-104 Admin</span>
        <span class="cert-box c-orange">AZ-900 Fdn</span>
      </td>
      <!-- GCP -->
      <td class="cert-cell">
        <span class="cert-box c-orange">Google IT Automation</span>
      </td>
      <!-- Java -->
      <td class="cert-cell">
        <span class="cert-box c-purple">OCA Java SE 8</span>
        <span class="cert-box c-purple">1Z0-808</span>
      </td>
      <!-- Python -->
      <td class="cert-cell">
        <span class="cert-box c-purple">PCEP (Python Inst)</span>
        <span class="cert-box c-purple">MS Python Dev</span>
      </td>
      <!-- SQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">Oracle SQL Assoc</span>
        <span class="cert-box c-green">1Z0-071</span>
      </td>
      <!-- NoSQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">MongoDB Python Dev</span>
      </td>
      <!-- DevOps -->
      <td class="cert-cell">
        <span class="cert-box c-red">Linux Foundation CKA</span>
      </td>
      <!-- Agile -->
      <td class="cert-cell">
        <span class="cert-box c-red">PSM I</span>
        <span class="cert-box c-red">CAPM</span>
      </td>
      <!-- Mobile -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Meta Android Dev</span>
      </td>
      <!-- Cross -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Salesforce Admin</span>
      </td>
    </tr>

    <tr>
      <td class="cert-cell" style="background:#f9f9f9; font-size:9px; color:#666; text-align:center;"></td>
      <!-- Frontend -->
      <td class="cert-cell">
        <span class="cert-box c-blue">fCC Front End Libs</span>
      </td>
      <!-- Full-Stack -->
      <td class="cert-cell">
        <span class="cert-box c-blue">The Odin Project</span>
      </td>
      <!-- AWS -->
      <td class="cert-cell">
        <span class="cert-box c-orange">AWS Cloud Practitioner</span>
      </td>
      <!-- Azure -->
      <td class="cert-cell">
        <span class="cert-box c-orange">PL-900 Power Platform</span>
      </td>
      <!-- GCP -->
      <td class="cert-cell">
        <span class="cert-box c-orange">Oracle OCI Fdn</span>
      </td>
      <!-- Java -->
      <td class="cert-cell">
        <span class="cert-box c-purple">Zend PHP Dev</span>
      </td>
      <!-- Python -->
      <td class="cert-cell">
        <span class="cert-box c-purple">DataCamp Data Sci</span>
      </td>
      <!-- SQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">MS Certified: Data</span>
      </td>
      <!-- NoSQL -->
      <td class="cert-cell">
        <span class="cert-box c-green">Cassandra Dev</span>
      </td>
      <!-- DevOps -->
      <td class="cert-cell">
        <span class="cert-box c-red">GitLab CI/CD Cert</span>
      </td>
      <!-- Agile -->
      <td class="cert-cell">
        <span class="cert-box c-red">Scrum.org PSM</span>
      </td>
      <!-- Mobile -->
      <td class="cert-cell">
        <span class="cert-box c-teal">Flutter Dev Cert</span>
      </td>
      <!-- Cross -->
      <td class="cert-cell">
        <span class="cert-box c-teal">HackerRank Skills</span>
      </td>
    </tr>

    <!-- BEGINNER ROW -->
    <tr>
      <td class="level-cell" style="background:#e8e8e8; writing-mode:vertical-lr; transform:rotate(180deg);">Başlanğıc</td>
      <td class="cert-cell" style="background:#f9f9f9; font-size:9px; color:#666; text-align:center;"></td>
      <!-- Frontend -->
      <td class="cert-cell">
        <span class="cert-box c-gray">fCC Responsive Web</span>
        <span class="cert-box c-gray">HTML/CSS Cert</span>
      </td>
      <!-- Full-Stack -->
      <td class="cert-cell">
        <span class="cert-box c-gray">IBM Full Stack (Coursera)</span>
        <span class="cert-box c-gray">CS50x Harvard</span>
      </td>
      <!-- AWS -->
      <td class="cert-cell">
        <span class="cert-box c-yellow">AWS Cloud Practitioner</span>
        <span class="cert-box c-yellow">CLF-C02</span>
      </td>
      <!-- Azure -->
      <td class="cert-cell">
        <span class="cert-box c-yellow">AZ-900</span>
        <span class="cert-box c-yellow">MS Fundamentals</span>
      </td>
      <!-- GCP -->
      <td class="cert-cell">
        <span class="cert-box c-yellow">Google Workspace Cert</span>
      </td>
      <!-- Java -->
      <td class="cert-cell">
        <span class="cert-box c-gray">Codecademy Java</span>
        <span class="cert-box c-gray">MOOC.fi Java</span>
      </td>
      <!-- Python -->
      <td class="cert-cell">
        <span class="cert-box c-gray">Google IT Auto Python</span>
        <span class="cert-box c-gray">Kaggle Python</span>
      </td>
      <!-- SQL -->
      <td class="cert-cell">
        <span class="cert-box c-gray">fCC Relational DB</span>
        <span class="cert-box c-gray">SQLZoo Cert</span>
      </td>
      <!-- NoSQL -->
      <td class="cert-cell">
        <span class="cert-box c-gray">MongoDB Basics</span>
      </td>
      <!-- DevOps -->
      <td class="cert-cell">
        <span class="cert-box c-gray">Git / GitHub Cert</span>
      </td>
      <!-- Agile -->
      <td class="cert-cell">
        <span class="cert-box c-gray">Scrum Intro</span>
        <span class="cert-box c-gray">Kanban Fdn</span>
      </td>
      <!-- Mobile -->
      <td class="cert-cell">
        <span class="cert-box c-gray">Codecademy Mobile</span>
      </td>
      <!-- Cross -->
      <td class="cert-cell">
        <span class="cert-box c-gray">Pccet (CompTIA)</span>
      </td>
    </tr>

  </tbody>
</table>
</div>

<p class="count-note">70+ sertifikat sıralanmışdır | Fevral 2026</p>

<p class="note">* Yuxarıda günümüzdə yaygın olaraq yer alan proqramlaşdırma dalları və bu dallarda etkin istifadə olunan sertifikatları görə bilərsiniz.</p>

<!-- ============ DETAIL SECTION ============ -->
<div class="detail-section">

  <h3>Veb İnkişafı (Web Development)</h3>
  <p>
    Frontend, Backend və Full-Stack sahələrini əhatə edir. HTML, CSS, JavaScript əsasları ilə başlayaraq React, Node.js, Django kimi freymvorklara qədər uzanır.
    <strong>freeCodeCamp</strong> sertifikatları tamamilə pulsuzdur. <strong>Meta Professional Certificates</strong> işəgötürənlər tərəfindən tanınan sertifikatlardır.
    Backend proqramçılar üçün <strong>JSNAD / JSNSD</strong> (Linux Foundation) Node.js üzrə ən tanınan rəsmi sertifikatlardır.
  </p>

  <h3>Bulud Hesablama (Cloud Computing)</h3>
  <p>
    AWS, Microsoft Azure və Google Cloud üzrə sertifikatlar proqramçılar üçün ən yüksək maaş artımını təmin edən sertifikat qrupudur.
    Başlanğıc üçün: <strong>AWS Cloud Practitioner (CLF-C02)</strong> ($100) və ya <strong>AZ-900 Azure Fundamentals</strong> (~$165) tövsiyə olunur.
    Orta səviyyə: <strong>AWS Developer Associate (DVA-C02)</strong> ($150). Ekspert: <strong>AWS Solutions Architect Professional</strong> ($300).
  </p>

  <h3>Java Proqramlaşdırması</h3>
  <p>
    Oracle tərəfindən verilən <strong>OCA Java SE 8 (1Z0-808)</strong> → <strong>OCP Java SE 17 (1Z0-829)</strong> yolu ən klassik Java sertifikat yoludur.
    Enterprise tərəf üçün <strong>Red Hat EX183</strong> əlavə edilə bilər. Java proqramçılarının qlobal ortalama maaşı ~$95,000-$150,000/il arasındadır.
  </p>

  <h3>Python / Data Science / AI</h3>
  <p>
    Python Institute-un <strong>PCEP → PCAP → PCPP</strong> sertifikat pilləsi tam strukturlu bir yol təklif edir.
    Data Science sahəsinə keçmək istəyənlər üçün <strong>Google IT Automation with Python</strong> (Coursera, ~$49/ay) ideal başlanğıc nöqtəsidir.
    AI/ML üçün isə <strong>TensorFlow Developer Certification</strong> ($100) və <strong>AWS ML Specialty</strong> ($300) tövsiyə olunur.
  </p>

  <h3>DevOps / Konteyner</h3>
  <p>
    <strong>Docker Certified Associate (DCA)</strong> ($400) → <strong>CKAD</strong> ($395) → <strong>CKA</strong> ($395) sırası DevOps karyerası üçün standart yoldur.
    Daha mürəkkəb mühitlər üçün <strong>CKS (Certified Kubernetes Security Specialist)</strong> əlavə edilə bilər.
    CI/CD sahəsində <strong>GitLab CI/CD Certification</strong> praktiki mənada çox dəyərlidir.
  </p>

  <h3>Verilənlər Bazası (Database)</h3>
  <p>
    SQL tərəf üçün <strong>Oracle SQL Certified Associate (1Z0-071)</strong> (~$245) ən populyar sertifikatlardandır.
    NoSQL tərəf üçün <strong>MongoDB Certified Developer Associate</strong> ($150) öndə gəlir.
    Böyük məlumat (Big Data) sahəsi üçün <strong>Databricks Apache Spark</strong> sertifikatı qiymətlidir.
  </p>

</div>

</body>
</html>
