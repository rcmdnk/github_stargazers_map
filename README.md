# GitHubのリポジトリにstarつけた人の住所をGoogleマイマップで出すやつ

## Setup
1. https://github.com/settings/tokens でアクセストークンを取得
2. [Google Maps Platform - Geo-location API Google Maps Platform  Google Cloud](https://cloud.google.com/maps-platform/?&_ga=2.198194155.575401857.1550238051-970206952.1525920064#get-started)からGoogle Maps API KEYを取得
2. `cp .env.example .env`
3. `.env` にアクセストークン/KEYを書くか環境変数で `export` する
4. `bundle install`

## Usage
```sh
bundle exec ruby github_stargazers_map.rb <user_name>/<repo_name>
```

`dist/` にKMLファイルが作られるのでGoogleマイマップにインポートする

# Example
https://github.com/sue445/jenkins-backup-script のstargazers map

https://drive.google.com/open?id=148eq4ySxjY5IQO_e29MkjMulfoI
