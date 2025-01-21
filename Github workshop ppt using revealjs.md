
<html>
<head>
 
  <title>Reveal.js Presentation</title>
  <link rel="stylesheet" href="https://unpkg.com/reveal.js/dist/reveal.css">
  <link rel="stylesheet" href="https://unpkg.com/reveal.js/dist/theme/black.css" id="theme">

  <style>
    
    h1, h2, h3, p, ul, blockquote, code {
      font-size: 17px; 
    }
  </style>

</head>
<body>
  <div class="reveal">
    <div class="slides">

      <!-- Slide 1 -->
      <section>
        <h1>📝 Daily Live Report (6 Months)</h1>
        <h2>📊 GitHub Workshop Report</h2>
        <p>📅 <strong>Date:</strong> 15/01/2025</p>
        <p>⏰ <strong>Start Time:</strong> 7:00 PM</p>
        <p>⏳ <strong>End Time:</strong> 9:00 PM</p>
      </section>

      <!-- Slide 2 -->
      <section>
        <h2>🔍 Learnings from the Workshop</h2>
        <h3>🌐 Version Control System & Git</h3>
        <ul>
          <li>Track changes made to files and create versions.</li>
          <li>Store metadata for each commit.</li>
          <li>Maintain a history of commits in a repository.</li>
          <li>Synchronize repositories across computers.</li>
          <li>Enable parallel work among team members.</li>
        </ul>
        <blockquote>
          💡 <strong>Note:</strong> Version control systems facilitate structured and efficient team collaboration.
        </blockquote>
      </section>

      <!-- Slide 3 -->
      <section>
        <h2>⚙️ Setting Up Git</h2>
        <p>Configurations required when using Git for the first time:</p>
        <ul>
          <li>Configuring user details:</li>
        </ul>
        <pre><code>
$ git config --global user.name "Your Name"
$ git config --global user.email "your.email@example.com"
        </code></pre>
        <p>Accessing help and manual:</p>
        <pre><code>
$ git config -h
$ git config --help
        </code></pre>
      </section>

      <!-- Slide 4 -->
      <section>
        <h2>📂 Creating a Repository</h2>
        <p>To create and initialize a Git repository:</p>
        <pre><code>
$ git init
        </code></pre>
        <h3>📜 Tracking Changes</h3>
        <p>Check project status:</p>
        <pre><code>
$ git status
        </code></pre>
        <blockquote>
          Example output:
          <pre><code>
On branch main
No commits yet
Untracked files:
   (use "git add <file>..." to include in what will be committed)
    filename
nothing added to commit but untracked files present (use "git add" to track)
          </code></pre>
        </blockquote>
        <p>Add a file to staging:</p>
        <pre><code>
$ git add filename
        </code></pre>
        <p>Commit changes:</p>
        <pre><code>
$ git commit -m "Your commit message"
        </code></pre>
      </section>

      <!-- Slide 5 -->
      <section>
        <h2>📌 Illustrative Diagram</h2>
        <p>Below is a basic representation of Git's workflow:</p>
        <img src="https://github.com/user-attachments/assets/639861d6-1306-49ab-aaf7-1a2f81d5fa62" alt="Git Workflow Diagram" style="width: 80%;">
      </section>

      <!-- Slide 6 -->
      <section>
        <h2>⚔️ Conflicts</h2>
        <p>Conflicts occur when two or more people change the same lines of the same file.</p>
        <p>Steps to resolve:</p>
        <ul>
          <li>Manually edit the conflicting files.</li>
          <li>Stage the resolved changes.</li>
          <li>Commit the resolution.</li>
        </ul>
      </section>

      <!-- Slide 7 -->
      <section>
        <h2>✅ Thank You!</h2>
        <p>To know more visit:</p>
        <p><a href="https://swcarpentry.github.io/git-novice/">GitHub workshop</a></p>
      </section>

    </div>
  </div>

  <script src="https://unpkg.com/reveal.js/dist/reveal.js"></script>
  <script>
    Reveal.initialize();
  </script>
</body>
</html>
