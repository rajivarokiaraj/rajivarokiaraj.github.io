<script src="https://app.launchdarkly.com/snippet/ldclient.min.js"></script>

<h1>Great Linked Learning</h1>
https://www.linkedin.com/learning-login/share?account=110408730&forceAccount=false&redirect=https%3A%2F%2Fwww.linkedin.com%2Flearning%2Fwhat-is-generative-ai%3Ftrk%3Dshare_ent_url%26shareId%3DhxEWKtePTQi22R1Sannutg%253D%253D


<div id="preview"style="display: none;">
  <h2>Preview</h2>
  <p>Click the button below to view the course on LinkedIn Learning.</p>
  <a href="https://www.linkedin.com/learning/what-is-generative-ai?trk=share_ent_url&shareId=hxEWKtePTQi22R1Sannutg%3D%3D" target="_blank" class="btn btn-primary">View Course</a>
<iframe
  width="100%"
  height="500"
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
    if (ldClient.variation('course-preview', false)) {
      document.getElementById('preview').style.display = 'block';
    }
  });
</script>