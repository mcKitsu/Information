# 伺服器公告

### <2020/09/11> - ZxyKira
因服務端完善度不足，決議預期釋出日改為為**2020/09/19**。

### <2020/09/04> - ZxyKira
開始伺服器公開計畫，預期釋放原味生存。預期釋出日為**2020/09/11**。


人的一生，是生不帶來死不帶去的一生。

我們在親人的歡笑聲中誕生，又在親人的悲傷中離去。

我們無法控制自己的生與死，多數人到了年邁的時候才能體會到健康長壽比榮華富貴更重要。

人就一生，我們都希望自己有個幸福的家，每天都是個快樂的人。

但在生活中，不是一切都盡人意，可是有什麼好看不開的？

煩惱憂愁，恩恩怨怨幾十年後都會隨生命而煙消雲散。

人的一生，只要我們不喪失對生活的信心，對理想的追求，做你想做的，愛你想愛的。

如果該奮鬥的去奮鬥了，該拼搏的去拼搏了，就能平常心看待得失：夢想是一時無法實現的，目標是短期難以達到的。

人的一生，不要去過份地苛求，不要有太多的奢望。既然上帝不偏愛於我，不讓我鶴立雞群，不讓我出類拔萃，又何必硬要去強求呢？

金錢、權力、名譽都不是最重要的，最重要的是善待自己，就算擁有了全世界，隨著死去也會煙消雲散。

人的一生，沒有事情是不可以放手的，我曾經以為，是不會放手一個人的。

其實，沒有什麼東西是不能放手的。

時日漸遠，當你回望，你會發現，你曾經以為不可以放手的東西，只是生命瞬間的一塊跳板。

所有的哀傷、痛楚，所有不能放棄的事情，不過是生命裡一個過渡。

失戀、失意，甚至失婚，以至我們在愛情裡所受的苦，都不過是一塊跳板，然而令你成長。

人的一生，開心也是一天，不開心也是一天，幹嗎硬要逼著自己不開心呢？

是啊，人就這麼一輩子，做錯事不可以重來的一輩子；碎了的心難再癒合的一輩子；過了今天就不會再有另一個今天的一輩子；一分一秒都不會再回頭的一輩子，我們為什麼不好好珍惜眼前，為什麼還要拼命地自怨自艾，痛苦追悔呢？

人的一生，我們可以淡然面對，也可以積極的把握，當你看不開、當你春風得意、當你憤憤不平、當你深陷痛苦中請想想它，不管怎麼樣，你總是幸運的擁有了這一輩子。

人的一生，沒有來世。所以讓我們從微笑開始！

人活一輩子，開心最重要。擁有健康的體魄，在快樂的心境中做自己喜歡做的事情，安然地實現自身價值，是人生最大的幸福。

# Dillinger

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Dillinger is a cloud-enabled, mobile-ready, offline-storage, AngularJS powered HTML5 Markdown editor.

  - Type some Markdown on the left
  - See HTML in the right
  - Magic

# New Features!

  - Import a HTML file and watch it magically convert to Markdown
  - Drag and drop images (requires your Dropbox account be linked)


You can also:
  - Import and save files from GitHub, Dropbox, Google Drive and One Drive
  - Drag and drop markdown and HTML files into Dillinger
  - Export documents as Markdown, HTML and PDF

Markdown is a lightweight markup language based on the formatting conventions that people naturally use in email.  As [John Gruber] writes on the [Markdown site][df1]

> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.

### Tech

Dillinger uses a number of open source projects to work properly:

* [AngularJS] - HTML enhanced for web apps!
* [Ace Editor] - awesome web-based text editor
* [markdown-it] - Markdown parser done right. Fast and easy to extend.
* [Twitter Bootstrap] - great UI boilerplate for modern web apps
* [node.js] - evented I/O for the backend
* [Express] - fast node.js network app framework [@tjholowaychuk]
* [Gulp] - the streaming build system
* [Breakdance](https://breakdance.github.io/breakdance/) - HTML to Markdown converter
* [jQuery] - duh

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

### Installation

Dillinger requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |


### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
