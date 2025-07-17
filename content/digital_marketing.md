---
title: "Digital Marketing"
date: 2025-07-12
draft: false
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="color-scheme" content="light only">
    <title>Document Viewer with Dropdown and Subtitle</title>
    <style>
        body {
            background-color: #f0f4f8;
            color: #002366;
            font-family: Arial, sans-serif;
            margin: 20px;
            text-align: center;
        }
        #subtitle {
            font-size: 1.25em;
            margin-top: 20px;
            color: #002366;
            text-align: center;
        }
        #content-display {
            width: 80%;
            margin: 10px auto;
        }
        iframe, video {
            width: 100%;
            height: 600px;
            border: 2px solid #ccc;
        }
        select {
            background-color: #002366;
            color: white;
            padding: 5px;
            border: 1px solid #ccc;
            font-size: 1em;
        }
        option {
            background-color: #002366;
            color: white;
        }
        @media (prefers-color-scheme: dark) {
            body {
                background-color: #f0f4f8 !important;
                color: #002366 !important;
            }
            #subtitle {
                color: #002366 !important;
            }
            select, option {
                background-color: #002366 !important;
                color: white !important;
            }
            #content-display {
                background-color: #ffffff !important;
            }
        }
    </style>
</head>
<body>

<h2>Google Certification</h2>

<div style="display: flex; justify-content: center; align-items: center; gap: 10px;">
  <select id="topicSelector" onchange="loadDocument(this)">
    <option value="">-- Select a topic --</option>
    <option value="/digital_marketing/topic_01.html" data-label="">01. Create Customer Personas</option>
    <option value="/digital_marketing/topic_02.html" data-label="">02. Improve Webpage Titles and Meta Descriptions</option>
    <option value="/digital_marketing/topic_03.html" data-label="">03. Create an Effective Response Search Ad </option>
    <option value="/digital_marketing/topic_04.html" data-label="">04. Optimize Responsive Ad Campaign</option>
    <option value="/digital_marketing/topic_05.html" data-label="">05. Create Social Media Campaign Calendar</option>
    <option value="/digital_marketing/topic_06.html" data-label="">06. Analyze Social Listening Data</option>
    <option value="/digital_marketing/topic_07.html" data-label="">07. Respond to Customer Comments</option>
    <option value="/digital_marketing/topic_08.mp4"  data-label="">08. Design a Social Media Post Using Canva</option>
    <option value="/digital_marketing/topic_09.html" data-label="">09. Analyze Social Media Performance</option>
    <option value="/digital_marketing/topic_10.html" data-label="">10. Analyze Social Media Performance</option>
    <option value="/digital_marketing/topic_11.html" data-label="">11. Create a Social Media Report Email</option>
    <option value="/digital_marketing/topic_12.html" data-label="">12. Create Social Media Ad Campaign</option>
    <option value="/digital_marketing/topic_13.html" data-label="">13. Write Subject Lines and Preview Text</option>
    <option value="/digital_marketing/topic_14.html" data-label="">14. Write a Retention Email</option>
    <option value="/digital_marketing/topic_15.html" data-label="">15. Write an Apology Email</option>
    <option value="/digital_marketing/topic_16.html" data-label="">16. Present Email Marketing Data to Stakeholders</option>
    <option value="/digital_marketing/topic_17.html" data-label="">17. Create SMART Goals for an Email Campaign</option>
    <option value="/digital_marketing/topic_18.html" data-label="">18. Segment an Email List</option>
    <option value="/digital_marketing/topic_19.html" data-label="">19. Complete an Email Series</option>
    <option value="/digital_marketing/topic_20.html" data-label="">20. Complete Email Campaign Presentation for Stakeholders</option>
    <option value="/digital_marketing/topic_21.html" data-label="">21. Set Performance Goals</option>
    <option value="/digital_marketing/topic_22.html" data-label="">22. Google Analytics Metrics</option>
    <option value="/digital_marketing/topic_23.html" data-label="">23. Create an Exploration in Google Analytics</option>
    <option value="/digital_marketing/topic_24.html" data-label="">24. Create Google Ad Recommendations</option>
    <option value="/digital_marketing/topic_25.html" data-label="">25. Explore Linked Data in Google Analytics</option>
    <option value="/digital_marketing/topic_26.html" data-label="">26. Make Campaign Budget Decisions</option>
    <option value="/digital_marketing/topic_27.html" data-label="">27. Plan an A/B Test</option>
    <option value="/digital_marketing/topic_28.html" data-label="">28. Complete Stakeholder Communication Plan</option>
    <option value="/digital_marketing/topic_29.html" data-label="">29. Sort and Filter Spreadsheet Data</option>
    <option value="/digital_marketing/topic_30.html" data-label="">30. Analyze Data Using Pivot Tables</option>
    <option value="/digital_marketing/topic_31.html" data-label="">31. Create Data Visualizations for Presentation</option>
    <option value="/digital_marketing/topic_32.html" data-label="">32. Present Data Insights to Stakeholders</option>
    <option value="/digital_marketing/topic_33.html" data-label="">33. Perform a Competitive Analysis</option>
    <option value="/digital_marketing/topic_34.html" data-label="">34. Identify Brand Values</option>
    <option value="/digital_marketing/topic_35.html" data-label="">35. Create a Mock e-Commerce Store with Shopify</option>
    <option value="/digital_marketing/topic_36.html" data-label="">36. Set Seasonal Budgets and Bids</option>
    <option value="/digital_marketing/topic_37.html" data-label="">37. Evaluate Checkout Process of eCommerce Store</option>
    <option value="/digital_marketing/topic_38.html" data-label="">38. Write a Customer Satisfaction Survey</option>
    <option value="/digital_marketing/topic_39.html" data-label="">39. Use Heat Map to Optimize a Landing Page</option>
    <option value="/digital_marketing/topic_40.html" data-label="">40. Suggest New Product Category Based on Search Data</option>
    <option value="/digital_marketing/topic_41.html" data-label="">41. Create an Internal Marketing Proposal</option>
    <option value="/digital_marketing/topic_42.html" data-label="">42. Adjust Campaign KeyWords</option>
    <option value="/digital_marketing/topic_43.html" data-label="">43. Create Marketing Report Presentation</option>
  </select>
</div>

<div id="subtitle"></div>

<div id="content-display"></div>

<script>
  function loadDocument(selectElement) {
    const selectedOption = selectElement.options[selectElement.selectedIndex];
    const url = selectedOption.value;
    const label = selectedOption.getAttribute('data-label') || '';
    const displayArea = document.getElementById('content-display');
    document.getElementById('subtitle').textContent = label;

    if (!url) {
      displayArea.innerHTML = `
        <img src="/digital_marketing/google_certification.jpg"
             style="display: block; margin: 0 auto; width: 100%; max-width: 1000px; height: auto; image-rendering: auto;"
             alt="Google Certification">`;
      return;
    }

    if (url.endsWith('.mp4')) {
      displayArea.innerHTML = `
        <video controls style="display: block; margin: 0 auto; max-width: 100%;">
          <source src="${url}" type="video/mp4">
          Your browser does not support the video tag.
        </video>`;
    } else if (url.endsWith('.jpg') || url.endsWith('.png') || url.endsWith('.jpeg') || url.endsWith('.gif') || url.endsWith('.webp')) {
      displayArea.innerHTML = `
        <img src="${url}"
             style="display: block; margin: 0 auto; width: 100%; max-width: 2000px; height: auto; image-rendering: auto;"
             alt="Loaded Image">`;
    } else {
      displayArea.innerHTML = `
        <iframe src="${url}" style="display: block; margin: 0 auto; width: 100%; height: 80vh; border: none;"></iframe>`;
    }
  }
</script>
</body>
</html>
