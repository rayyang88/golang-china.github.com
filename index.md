---
layout: default
---

{{ range .site.posts.Top5 }}
<article>
	<h1>{{ .title }}</h1>
	<cite>Posted by <a href="{{ .authorlink }}" target="_blank">{{ .author }}</a> on {{ .date | date_to_string }}</cite>
	{{ .content }}
</article>
{{ end }}

