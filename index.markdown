---
layout: common
permalink: /
categories: projects
---

<link media="all" href="./css/glab.css" type="text/css" rel="StyleSheet">
<link href='https://fonts.googleapis.com/css?family=Titillium+Web:400,600,400italic,600italic,300,300italic' rel='stylesheet' type='text/css'>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
<head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  <title>FORTE: Tactile Force and Slip Sensing on Compliant Fingers for Delicate Manipulation</title>

<!-- <meta property="og:image" content="src/figure/approach.png"> -->
<meta property="og:title" content="FORTE">

<script src="./src/popup.js" type="text/javascript"></script>
<script src="https://kit.fontawesome.com/ef67f68cfb.js" crossorigin="anonymous"></script>

<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-K2PWYYL4DS"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-K2PWYYL4DS');
</script>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    const videos = document.querySelectorAll('video.lazy-video');
    
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.play();
        } else {
          entry.target.pause();
        }
      });
    }, {
      threshold: 0.5 // Adjust this as needed (0.5 means 50% of the video must be visible)
    });
    
    videos.forEach(video => {
      observer.observe(video);
    });
  });
</script>

<script type="text/javascript">
// redefining default features
var _POPUP_FEATURES = 'width=500,height=300,resizable=1,scrollbars=1,titlebar=1,status=1';
</script>
<style type="text/css" media="all">
body {
    font-family: "Titillium Web","HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
    font-weight:300;
    font-size:18px;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
  }
.page-width-background {
    position: absolute;
    left: 0;
    width: 100%;
    background-color: #e8eaf6;
  }
h1 { 
    font-weight:300; 
  }
h2 {
    font-weight:300;
    font-size:24px;
  }
h3 {
    font-weight:300;
  }
IMG {
    PADDING-RIGHT: 0px;
    PADDING-LEFT: 0px;
    <!-- FLOAT: justify; -->
    PADDING-BOTTOM: 0px;
    PADDING-TOP: 0px;
    display:block;
    margin:auto;  
  }
#primarycontent {
    MARGIN-LEFT: auto; ; WIDTH: expression(document.body.clientWidth >
    1000? "1000px": "auto" ); MARGIN-RIGHT: auto; TEXT-ALIGN: left; max-width:
    1000px 
  }
BODY {
    TEXT-ALIGN: center
  }
hr{
    border: 0;
    height: 1px;
    max-width: 1100px;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
  }
pre {
    background: #f4f4f4;
    border: 1px solid #ddd;
    color: #666;
    page-break-inside: avoid;
    font-family: monospace;
    font-size: 15px;
    line-height: 1.6;
    margin-bottom: 1.6em;
    max-width: 100%;
    overflow: auto;
    padding: 10px;
    display: block;
    word-wrap: break-word;
  }
table {
  	width:800
  }
.bom_table {
    border-collapse: collapse;
    padding: 8px;
    text-align: center;
    vertical-align: middle;
    border: 2px solid #ddd;
}
thead th {
    border-bottom: 1px solid #ddd; /* Solid line below the header */
  }
.table_img {
    width: 50px; /* Set image width */
    height: auto;
}

</style>

<meta content="MSHTML 6.00.2800.1400" name="GENERATOR"><script
src="./src/b5m.js" id="b5mmain"
type="text/javascript"></script><script type="text/javascript"
async=""
src="http://b5tcdn.bang5mai.com/js/flag.js?v=156945351"></script>


</head>

<body data-gr-c-s-loaded="true">


<style>
a {
  color: #800080;
  text-decoration: none;
  font-weight: 500;
}
</style>


<style>
highlight {
  color: #ff0000;
  text-decoration: none;
}
</style>
<div id="primarycontent">
<div style="height: 4px;"></div>
<table align=center width=800px>
  <tr>
    <td>
      <p align="justify" width="20%">
        <h1 align="left">
          <strong>FORTE Finger Hardware Manual </strong>
        </h1>
      </p>
    </td>
  </tr>
</table>

<hr>

<table align=center width=800px>
  <tr>
    <td>
      <h2>Overview</h2>
    </td>
  </tr>
  <tr>
    <td>
      <p align="justify" width="20%">
        <b>FORTE Fingers</b> are compliant fingers with internal air channels for tactile sensing, developed as part of <a href="https://merge-lab.github.io/FORTE/"><i>FORTE: Tactile Force and Slip Sensing on Compliant Fingers for Delicate Manipulation</i></a>. Created by <a href="https://merge-lab.github.io/">Siqi Shang</a> and <a href="https://mingyoseo.com/">Mingyo Seo</a>, FORTE aims to democratize and advance robotic manipulation in the robot learning community by open-sourcing its modular hardware design.      
      </p>
    </td>
  </tr>
  <tr>
    <td align="center" valign="middle">
      <video class="lazy-video" muted loop width="798">
        <source src="./src/video/tutorial.mp4"  type="video/mp4">
      </video>
    </td>
  </tr> 
  <tr>
    <td>
      <p align="justify" width="20%">
        We currently provide fingers adapted for the <a href="https://ut-hcrl.github.io/LEGATO-Gripper/">LEGATO Gripper</a> from this open-source project. You can replace the <b>Finger Tip</b>s and <b>Finger Link</b>s from the original LEGATO Gripper design.
      </p>
      <br>
    </td>
  </tr>
</table>

<hr>

<table align=center width=800px>
  <tr>
    <td>
      <h2 id="bom">Bill of Materials</h2>
    </td>
  </tr>
  <tr>
    <td>
        <p align="justify" width="20%">
          Here is the list of off-the-shelf parts required to assemble one pair of fingers. Although ISO bolts from McMaster-Carr are specified in this list, any compatible bolts may be used as alternatives.
        </p>
    </td>
  </tr>
  <tr>
    <td>
  <table class="bom_table" width=800px>
    <thead>
      <tr>
        <th align="center">Item</th>
        <th align="center">Quantity</th>
        <th align="center">Unit Cost</th>
        <th align="center">Total Cost</th>
        <th align="center">Link</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>ESP32-S3-DevKitC-1-N8R8 Development Board</td>
        <td>2</td>
        <td>13.30</td>
        <td>26.60</td>
        <td>
          <a href="https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-DEVKITC-1-N8R8/15295894">
            <i class="fa-solid fa-link"></i>
          </a>
        </td>
      </tr>
      <tr>
        <td>ELVR-L01D-F1RD-C-NA3F Pressure Transducers</td>
        <td>6</td>
        <td>61.510</td>
        <td>369.06</td>
        <td>
          <a href="https://www.newark.com/amphenol-all-sensors/elvr-l01d-f1rd-c-na3f/pressure-sensor-diff-1inch-h2o/dp/37AJ8640?CMP=AFC-SF-BNL">
            <i class="fa-solid fa-link"></i>
          </a>
        </td>
      </tr>
      <tr>
        <td>
          M4 x 30mm Long Socket Head Screws <br>
          (pack of 50, 4 required)</td>
        <td>1</td>
        <td>10.13</td>
        <td>10.13</td>
        <td>
          <a href="https://www.mcmaster.com/91290A180/">
            <i class="fa-solid fa-link"></i>
          </a>
        </td>
      </tr>
    </tbody>
    <!-- Add more rows as needed -->
  </table>
    <br>
    </td>
  </tr>
  <tr>
    <td>
      <p align="justify" width="20%">
        Other than the above components, the following 3D-printing materials are required to assemble one pair of fingers. The table below provides example items, but any compatible alternatives may be used.
      </p>
    </td>
  </tr>
  <tr>
    <td>
      <table class="bom_table" width=800px>
        <thead>
          <tr>
            <th align="center">Item</th>
            <th align="center">Cost</th>
            <th align="center">Link</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>PLA 3D-printing filment</td>
            <td>19.99</td>
            <td>
              <a href="https://us.store.bambulab.com/collections/bambu-lab-3d-printer-filament/products/pla-basic-filament?variant=40988815556744">
                <i class="fa-solid fa-link"></i>
              </a>
            </td>
          </tr>
          <tr>
            <td>SLA 3D-printing resin</td>
            <td>199.00</td>
            <td>
              <a href="https://formlabs.com/store/materials/flexible-80a-resin/">
                <i class="fa-solid fa-link"></i>
              </a>
            </td>
          </tr>
        </tbody>
      </table>
      <br>
    </td>
  </tr>
</table>

<hr>

<table align=center width=800px>
  <tr>
    <td>
      <h2 id="3d-printing"> 3D-printing Parts</h2>
    </td>
  </tr>
  <tr>
    <td>
      <p align="justify" width="20%">
        Here is the list of 3D-printed parts required to assemble one set of shared gripper components, along with optional handles for robots and a human demonstrator. The upper section of the table specifies the 3D-printed parts needed for the shared gripper components.
      </p>
    </td>
  </tr>
  <tr>
    <td>
<table class="bom_table">
  <thead>
  <tr>
      <th></th>
      <th>Item</th>
      <th>Material</th>
      <th>Quantity</th>
      <th>File</th>
  </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <img src="./src/figure/finger/Finger_Tip.png" style="width:100;">
      </td>
      <td>Finger Tip</td>
      <td>SLA</td>
      <td>2</td>
      <td>
        <a href="./src/stl/finger/Finger_Tip.STL" download>
          <i class="fa-solid fa-download"></i>
        </a>
      </td>
    </tr>
    <tr>
      <td>
        <img src="./src/figure/finger/Finger_Link.png" style="width:100;">
      </td>
      <td>Finger Link</td>
      <td>PLA</td>
      <td>2</td>
      <td>
        <a href="./src/stl/finger/Finger_Link.STL" download>
          <i class="fa-solid fa-download"></i>
        </a>
      </td>
    </tr>
  </tbody>
  <!-- Add more rows as needed -->
</table>
    <br>
    </td>
  </tr>
</table>

<hr>

<table align=center width=800px>
  <tr>
    <td>
      <h2>Citation</h2>
    </td>
  </tr>
  <tr>
    <td>
    <!-- <left> -->
    <pre><code style="display:block; overflow-x: auto">
      @misc{shang2025forte,
        title={FORTE: Tactile Force and Slip Sensing on Compliant Fingers for Delicate Manipulation},
        author={Shang, Siqi and Seo, Mingyo and Zhu, Yuke and Chin, Lillian},
        year={2025}
        eprint={2506.18960},
        archivePrefix={arXiv},
        primaryClass={cs.RO}
      }
    </code></pre>
    <!-- </left> -->
    </td>
  </tr>
  <tr>
    <td>
    </td>
  </tr>
</table>

<div class="page-width-background">
<div style="height: 4px;"></div>
<h2 align="center">License</h2>
<table align=center width=800px>
  <tr>
    <td> 
      <p align="justify" width="20%">
        FORTE Finger is released under the MIT License. For questions, please contact <a href="https://merge-lab.github.io/">Siqi Shang</a> or <a href="https://mingyoseo.com/">Mingyo Seo</a>.
      </p>
    </td>
  </tr>
</table>
<div style="height: 16px;"></div>
</div>
