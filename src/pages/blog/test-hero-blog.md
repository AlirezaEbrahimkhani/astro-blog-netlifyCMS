---
layout: ../../layouts/BlogPost.astro
title: Test Hero Blog
description: Test Hero Blog Description
pubDate: 2022-09-15T12:33:35.737Z
heroImage: /assets/placeholder-social.jpg
---
Here is a sample of some basic Markdown syntax that can be used when writing Markdown content in Astro.

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

![Salon Background](/assets/salon-bg.png)



```abuild
const assets = await Astro.glob('../assets/**/*');
const heroImageAsset = assets.find(asset => {
	if (!heroImage) {
		return false;
	}
  	if (!asset.default?.src) {
		return false;
	}
  	const index = asset.default.src.indexOf('/assets/');
  	return asset.default.src.slice(index) === heroImage;
});
```