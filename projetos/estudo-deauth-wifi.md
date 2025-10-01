<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>{{ page.title | default: site.title }}</title>
  <meta name="description" content="{{ page.description | default: site.description }}" />
  <link rel="stylesheet" href="{{ '/assets/style.css' | relative_url }}">
</head>
<body>
  <header class="site-header">
    <div class="container">
      <a href="{{ '/' | relative_url }}" class="brand">{{ site.title }}</a>
      <nav class="main-nav">
        <a href="{{ '/' | relative_url }}">Home</a>
        <a href="{{ '/deauth.html' | relative_url }}">Deauth Study</a>
        <a href="{{ '/projects' | relative_url }}">Projetos</a>
      </nav>
    </div>
  </header>

  <main class="container">
    {{ content }}
  </main>

  <footer class="site-footer">
    <div class="container">
      <p>© {{ site.title }} — {{ site.author | default: "Seu Nome" }}</p>
    </div>
  </footer>
</body>
</html>
