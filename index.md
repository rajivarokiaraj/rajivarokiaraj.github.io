<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Great Linked Learning</title>
  <script src="https://app.launchdarkly.com/snippet/ldclient.min.js"></script>
  <style>
    body {
      font-family: sans-serif;
      padding: 20px;
    }

    .btn {
      display: inline-block;
      padding: 10px 20px;
      background-color: #0073b1;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }

    .btn:hover {
      background-color: #005582;
    }
  </style>
</head>
<body>

  <h1>Great Linked Learning</h1>
  <p>🔗 Direct Course Link: 
    <a href="https://www.linkedin.com/learning/what-is-generative-ai?trk=share_ent_url&shareId=hxEWKtePTQi22R1Sannutg%3D%3D" target="_blank">
      What is Generative AI
    </a>
  </p>

  <div id="preview" style="display: none;">
    <h2>🎓 Preview Available</h2>
    <p>Click below to view the full course on LinkedIn Learning:</p>
    <a href="https://www.linkedin.com/learning/what-is-generative-ai?trk=share_ent_url&shareId=hxEWKtePTQi22R1Sannutg%3D%3D" target="_blank" class="btn">▶️ View Course</a>
    
    <h3>📺 Sample 4K Video</h3>
    <iframe
      width="100%"
      height="400"
      src="https://www.youtube.com/embed/sQ22pm-xvrE"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    ></iframe>
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
