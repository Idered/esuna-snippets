# esuna-snippets

Sublime Text snippets for [Esuna Framework](http://idered.pl/esuna)

## Instalation

**Using Package Control**

This method is curently not available but soon, it'll be.

**Manual instalation**

[Download](https://github.com/Idered/esuna-snippets/archive/master.zip) this repo. In Sublime Text go to: Preferences->Browse Packages... Create there new folder called <code>Esuna Framework Snippets</code> and paste downloaded archive content.


## Snippets

**esuna-comment1**

```CSS


/** $1 */
/*---------------------------------------------------------------------------*/

$2
```


**esuna-comment2**

```CSS

/** ${1:%|=}${2:[$3]} $4 */
/*------------------------------------*/
$5
```


**esuna-comment3**

```CSS

/*------------------------------------*/

$1
```


**esuna-open-graph**

```CSS
<!-- @see ogp.me -->
<meta name="og:title" content="$1" />
<meta name="og:type" content="${2:website}" />
<meta name="og:description" content="$3" />
<meta name="og:url" content="$4">
```


**esuna-twitter-card**

```CSS
<!-- @see dev.twitter.com/docs/cards -->
<meta name="twitter:card" content="${1:summary}">
<meta name="twitter:creator" content="@$2">
<meta name="twitter:site" content="@$3">
<meta name="twitter:url" content="$4">
<meta name="twitter:title" content="$5">
<meta name="twitter:description" content="$6">
```


**esuna-dns-prefetch**

```CSS
<!-- @see developer.mozilla.org/en-US/docs/Controlling_DNS_prefetching -->
<link rel="dns-prefetch" href="//p.twitter.com">
<link rel="dns-prefetch" href="//cdn.api.twitter.com">
<link rel="dns-prefetch" href="//ajax.googleapis.com">
<link rel="dns-prefetch" href="//fonts.googleapis.com">
<link rel="dns-prefetch" href="//connect.facebook.net">
<link rel="dns-prefetch" href="//platform.twitter.com">
```


**esuna-load-scripts**

```CSS
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
