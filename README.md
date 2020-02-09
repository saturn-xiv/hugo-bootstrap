# Bootstrap theme for hugo

## Usage

```bash
$ git submodule add https://github.com/saturn-xiv/hugo-bootstrap.git themes/bootstrap
$ cp themes/bootstrap/package.json themes/bootstrap/exampleSite/config.toml themes/bootstrap/.gitignore ./
# install third dependicies
$ npm install
# run server
$ hugo server -D
# build site
$ hugo -D --minify
```

## Deployment by rsync

```bash
$ rsync -avz --delete public/ deploy@www.examples.com:/var/www/www.examples.com/htdocs
```

## Nginx

```nginx
server {
    server_name www.examples.org;
    root /var/www/www.examples.org/htdocs;
    index index.html;
}
```

## Documents

- [Bootstrap](https://getbootstrap.com/)
- [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)
- [config.toml](https://github.com/saturn-xiv/hugo-bootstrap/blob/master/exampleSite/config.toml)
