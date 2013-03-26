# esuna-snippets

Sublime Text snippets for [Esuna Framework](http://idered.pl/esuna)

**esuna-comment1**

```


/** $1
/*---------------------------------------------------------------------------*/

$2
```

**esuna-comment2**

```

/** ${1:%|=}${2:[$3]} $4 */
/*------------------------------------*/
$5
```

**esuna-comment3**

```

/*------------------------------------*/

$1
```

**esuna-open-graph**

```
<!-- @see ogp.me -->
<meta property="og:title" content="$1" />
<meta property="og:type" content="${2:website}" />
<meta property="og:description" content="$3" />
<meta property="og:url" content="$4">
```

**esuna-twitter-card**

```
<!-- @see dev.twitter.com/docs/cards -->
<meta property="twitter:title" content="$1">
<meta property="twitter:creator" content="@$2">
<meta property="twitter:card" content="${3:summary}">
<meta property="twitter:description" content="$4">
<meta property="twitter:url" content="$5">
```

**esuna-dns-prefetch**

```
<!-- @see developer.mozilla.org/en-US/docs/Controlling_DNS_prefetching -->
<link rel="dns-prefetch" href="//p.twitter.com">
<link rel="dns-prefetch" href="//cdn.api.twitter.com">
<link rel="dns-prefetch" href="//ajax.googleapis.com">
<link rel="dns-prefetch" href="//fonts.googleapis.com">
<link rel="dns-prefetch" href="//connect.facebook.net">
<link rel="dns-prefetch" href="//platform.twitter.com">
```

**esuna-load-scripts**

```
<div id="fb-root"></div>
<script>
	var scripts = {
		'facebook-jssdk': '//connect.facebook.net/en_US/all.js#xfbml=1',
		'googleplus'    : 'https://apis.google.com/js/plusone.js',
		'twitter-wjs'   : '//platform.twitter.com/widgets.js',
		'analytics'     : ('https:'==location.protocol?'//ssl':'//www') + '.google-analytics.com/ga.js'
	}, script, _gaq=[['_setAccount','UA-XXXXX-X'],['_trackPageview']];

	for (var id in scripts) {
		script = document.createElement('script'); script.src = scripts[id];
		script.id = id;script.type = 'text/javascript'; script.async = true;
		document.getElementsByTagName('head')[0].appendChild(script);
	}
</script>
```
