<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Great Linked Learning – rajivarokiaraj</title>
  <style>
    .btn {
      display: inline-block;
      padding: 10px 20px;
      background-color: #0073b1;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      margin-top: 10px;
    }
    .btn:hover {
      background-color: #005582;
    }
  </style>
</head>
<body>

  <h1>Great Linked Learning – rajivarokiaraj</h1>

  <p>Direct Course Link:</p>
  <a href="https://www.linkedin.com/learning-login/share?account=110408730&forceAccount=false&redirect=https%3A%2F%2Fwww.linkedin.com%2Flearning%2Fwhat-is-generative-ai%3Ftrk%3Dshare_ent_url%26shareId%3DhxEWKtePTQi22R1Sannutg%253D%253D" 
     target="_blank">
     What is Generative AI (LinkedIn Learning)
  </a>

  <div id="preview" style="display: none; margin-top: 20px;">
    <h2>🎓 Preview</h2>
    <p>Click the button below to view the course on LinkedIn Learning.</p>
    <a class="btn" 
       href="https://www.linkedin.com/learning/what-is-generative-ai?trk=share_ent_url&shareId=hxEWKtePTQi22R1Sannutg%3D%3D" 
       target="_blank">
       ▶️ View Course
    </a>
  </div>




  <script>
    // Initialize LaunchDarkly
    const ldClient = LDClient.initialize('6842e842905004094bb0f4d5', {
      key: 'course-preview',
      anonymous: true
    });

    // Check when LD is ready
    ldClient.on('ready', function() {
      const showPreview = ldClient.variation('course-preview', false);
      if (showPreview) {
        document.getElementById('preview').style.display = 'block';
      }
    });
  </script>

</body>
</html>
