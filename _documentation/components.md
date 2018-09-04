---
title: Components
collection_id: components
---

# {{page.title}}

An Origami component is a collection of styles and functionality. It provides reusable <abbr title="Hypertext Markup Language">HTML</abbr>, <abbr title="Sassy Cascading Style Sheets">SCSS</abbr> and JavaScript for a multitude of different products under the <abbr title="Financial Times">FT</abbr> umbrella.

## Building your component

Origami components need to be 'built' before they are delivered to a browser.

How you choose to do this will depend on your projects' requirements, so there are a couple of ways in which you can set it all up.

- Using the Origami Build Service:  
	The Build service is best for quick projects or static sites or things where performance is less of a concern. This build method will fetch the Origami <abbr title="Cascading Style Sheets">CSS</abbr> and JavaScript as external files for your webpage. Be aware that this will indiscriminately fetch all stylistic variations of a component, which will increase your file size.


	If you would like help with this, you can visit the [Build Service tutorial](/tutorials/build-service/)


- Using the manual build process:  
	In order to customise your page and have more granular control over a components stylistic and behavioural features, you'll want to build Origami components manually. We currently do this with Bower, and install Origami components from the command line. This process relies on a build step, which you may already have in your project. If not, the <a href="https://github.com/Financial-Times/origami-build-tools" class="o-typography-link--external" target="\_blank" rel="noopener">Origami Build Tools</a> provide one.  


	If you would like help with this, you can visit the [manual build tutorial](/tutorials/manual-build/)

- Building branded components  
	brandbrandbrand  
	[Branding tutorial](/TODO).

## Documentation
<ul>
	{% for item in site[page.collection_id] %}
		<li>
			<a href="{{item.url}}">{{item.title}}</a>
		</li>
	{% endfor %}
</ul>