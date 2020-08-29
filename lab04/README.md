# Serviços

## Tarefa 01
> ![Diagrama de Orquestração](images/tarefa01.png)
## Tarefa 02
> ![Diagrama de Orquestração](images/tarefa02.png)
## Tarefa 03
> ![Diagrama de Orquestração](images/tarefa03.png)
## Tarefa 04

### Serviço `<Skyscanner Flight Search>`

* **Título do serviço**: `Skyscanner Flight Search`
* **Breve descrição**:
  > Permite procurar por voos e preços da base de dados.
* **URL completa da requisição**: `https://rapidapi.p.rapidapi.com/__test`
* **Cabeçalho HTTP da chamada**:
~~~http
POST /__test HTTP/1.1
Host: rapidapi.p.rapidapi.com
Connection: keep-alive
Content-Length: 2232
rate: 4.146985
locale: en-US
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
Content-Type: application/json
Accept: application/json, text/plain, */*
symbol: R$
x-entity-id: 4692814
country: BR
brand: default
csrf-token: 
Origin: https://rapidapi.com
Sec-Fetch-Site: same-site
Sec-Fetch-Mode: cors
Sec-Fetch-Dest: empty
Referer: https://rapidapi.com/skyscanner/api/skyscanner-flight-search?endpoint=5a9c9edde4b084deb4ea6195
Accept-Encoding: gzip, deflate, br
Accept-Language: pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7
~~~
* **Cabeçalho HTTP da resposta**:
~~~http
HTTP/1.1 200 OK
Access-Control-Allow-Origin: *
Content-Encoding: gzip
Content-Type: application/json; charset=utf-8
Date: Sat, 29 Aug 2020 00:24:30 GMT
ETag: W/"6f1-bMECmZR7WAshevhb6ARmtb7EwLE"
Server: openresty/1.13.6.1
Vary: Accept-Encoding
X-Powered-By: Express
Content-Length: 551
Connection: keep-alive
~~~
* **Conteúdo da resposta**:
~~~json
{
    "body": 
    {
        "Places": 
        [            
            {
                "PlaceId": "SAOA-sky",
                "PlaceName": "São Paulo",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "SAOA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "GRU-sky",
                "PlaceName": "Sao Paulo Guarulhos",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "SAOA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "CGH-sky",
                "PlaceName": "São Paulo Congonhas",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "SAOA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "VCP-sky",
                "PlaceName": "São Paulo Viracopos",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "SAOA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "SJP-sky",
                "PlaceName": "São José do Rio Preto",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "SJPA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "SJK-sky",
                "PlaceName": "São José Dos Campos",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "SJKA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "RAO-sky",
                "PlaceName": "Ribeirão Preto",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "RAOA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "PPB-sky",
                "PlaceName": "Presidente Prudente",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "PPBA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "ARU-sky",
                "PlaceName": "Araçatuba",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "ARUA-sky",
                "CountryName": "Brasil"
            },            
            {
                "PlaceId": "BAUA-sky",
                "PlaceName": "Bauru",
                "CountryId": "BR-sky",
                "RegionId": "",
                "CityId": "BAUA-sky",
                "CountryName": "Brasil"
            }
        ]
    },
    "headers": 
    {
        "cache-control": "max-age=0,no-cache,no-store,must-revalidate,post-check=0,pre-check=0",
        "content-type": "application/json",
        "date": "Sat, 29 Aug 2020 00:24:30 GMT",
        "expires": "Thu, 27 Aug 2020 00:24:29 GMT",
        "pragma": "no-cache",
        "server": "RapidAPI-1.1.24",
        "vary": "*",
        "x-rapidapi-region": "AWS - sa-east-1",
        "x-rapidapi-version": "1.1.24",
        "x-skyscnr-expr-e": "true",
        "content-length": "1326",
        "connection": "Close"
    },
    "statusCode": 200,
    "error": false
}
~~~

### Serviço `<Spotify>`

* **Título do serviço**: `<Spotify>`
* **Breve descrição**:
  > Buscar músicas a qualquer hora, em qualquer lugar.
* **URL completa da requisição**: `<https://any-api.com:8443/https://api.spotify.com/v1/me/tracks?limit=1&offset=0&market=BR>`
* **Cabeçalho HTTP da chamada**:
~~~http
GET /https://api.spotify.com/v1/me/tracks?limit=1&offset=0&market=BR
Host: any-api.com:8443
:scheme: https
accept: */*
accept-encoding: gzip, deflate, br
accept-language: pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7
authorization: Bearer BQByJyvwQZqiRfWSrrO-M7m0mkNls8GEpgVnTF8lAn_WbqxY1YT0YRqi0NN4egMn4nd0Ie2HFMsvbSgKJLZif8tDypw5k46M5aY3DuVxCp1uGxDkrEy8WYsKhOYtxpRa6aGNt-Vn9gWkNr78mDkgagc_ncccqQxNSbPUmAGMKck2GPDoCMTM-ri4PFTVSrMnxiPuCMOuGkClSpCeS_lQLlz44RLwxtk128wIldTi1xHRLKLpM9vFbSSbrooFIjzM2_0
if-none-match: W/"MC-Ijc4YjRmNzE0MGUwODI3YTRmYzc0MGEwNmFiNDAxNTY3Ig=="
origin: https://any-api.com
referer: https://any-api.com/spotify_com/spotify_com/console/_me_tracks/GET
sec-fetch-dest: empty
sec-fetch-mode: cors
sec-fetch-site: same-site
user-agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
~~~
* **Cabeçalho HTTP da resposta**:
~~~http
access-control-allow-credentials: true
access-control-allow-headers: Accept, App-Platform, Authorization, Content-Type, Origin, Retry-After, Spotify-App-Version, X-Cloud-Trace-Context
access-control-allow-methods: GET, POST, OPTIONS, PUT, DELETE, PATCH
access-control-allow-origin: *
access-control-expose-headers: content-type,cache-control,etag,vary,x-robots-tag,access-control-allow-origin,access-control-allow-headers,access-control-allow-methods,access-control-allow-credentials,access-control-max-age,content-encoding,strict-transport-security,x-content-type-options,date,server,via,alt-svc,connection,transfer-encoding,x-final-url
access-control-max-age: 604800
cache-control: private, max-age=0
cf-cache-status: DYNAMIC
cf-ray: 5ca235eebc98eec6-GRU
cf-request-id: 04d94009320000eec63abc1200000001
content-encoding: br
content-type: application/json; charset=utf-8
date: Sat, 29 Aug 2020 00:38:42 GMT
etag: W/"MC-Ijc4YjRmNzE0MGUwODI3YTRmYzc0MGEwNmFiNDAxNTY3Ig=="
expect-ct: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
server: cloudflare
set-cookie: __cfduid=dc7da9503139047be065c5be29dc3faf91598661521; expires=Mon, 28-Sep-20 00:38:41 GMT; path=/; domain=.any-api.com; HttpOnly; SameSite=Lax
status: 200
strict-transport-security: max-age=31536000
vary: Authorization
via: HTTP/2 edgeproxy, 1.1 google
x-content-type-options: nosniff
x-final-url: https://api.spotify.com/v1/me/tracks?limit=1&offset=0&market=BR
x-request-url: https://api.spotify.com/v1/me/tracks?limit=1&offset=0&market=BR
x-robots-tag: noindex, nofollow
~~~
* **Conteúdo da resposta**:
~~~json
{
  "href" : "https://api.spotify.com/v1/me/tracks?offset=0&limit=1&market=BR",
  "items" : [ {
    "added_at" : "2020-08-25T01:03:52Z",
    "track" : {
      "album" : {
        "album_type" : "single",
        "artists" : [ {
          "external_urls" : {
            "spotify" : "https://open.spotify.com/artist/4vxaQs6vK54nK89J1VtLex"
          },
          "href" : "https://api.spotify.com/v1/artists/4vxaQs6vK54nK89J1VtLex",
          "id" : "4vxaQs6vK54nK89J1VtLex",
          "name" : "PUBLIC",
          "type" : "artist",
          "uri" : "spotify:artist:4vxaQs6vK54nK89J1VtLex"
        } ],
        "external_urls" : {
          "spotify" : "https://open.spotify.com/album/2CxrZinzjDXZidyx5EP214"
        },
        "href" : "https://api.spotify.com/v1/albums/2CxrZinzjDXZidyx5EP214",
        "id" : "2CxrZinzjDXZidyx5EP214",
        "images" : [ {
          "height" : 640,
          "url" : "https://i.scdn.co/image/ab67616d0000b2730d0621554b1c6c9dbf3556be",
          "width" : 640
        }, {
          "height" : 300,
          "url" : "https://i.scdn.co/image/ab67616d00001e020d0621554b1c6c9dbf3556be",
          "width" : 300
        }, {
          "height" : 64,
          "url" : "https://i.scdn.co/image/ab67616d000048510d0621554b1c6c9dbf3556be",
          "width" : 64
        } ],
        "name" : "Make You Mine",
        "release_date" : "2019-08-09",
        "release_date_precision" : "day",
        "total_tracks" : 3,
        "type" : "album",
        "uri" : "spotify:album:2CxrZinzjDXZidyx5EP214"
      },
      "artists" : [ {
        "external_urls" : {
          "spotify" : "https://open.spotify.com/artist/4vxaQs6vK54nK89J1VtLex"
        },
        "href" : "https://api.spotify.com/v1/artists/4vxaQs6vK54nK89J1VtLex",
        "id" : "4vxaQs6vK54nK89J1VtLex",
        "name" : "PUBLIC",
        "type" : "artist",
        "uri" : "spotify:artist:4vxaQs6vK54nK89J1VtLex"
      } ],
      "disc_number" : 1,
      "duration_ms" : 232906,
      "explicit" : false,
      "external_ids" : {
        "isrc" : "TCACE1578479"
      },
      "external_urls" : {
        "spotify" : "https://open.spotify.com/track/5iFwAOB2TFkPJk8sMlxP8g"
      },
      "href" : "https://api.spotify.com/v1/tracks/5iFwAOB2TFkPJk8sMlxP8g",
      "id" : "5iFwAOB2TFkPJk8sMlxP8g",
      "is_local" : false,
      "is_playable" : true,
      "name" : "Make You Mine",
      "popularity" : 84,
      "preview_url" : "https://p.scdn.co/mp3-preview/b03175563bf8617fb5ee6b8e22730ba9a21eec8d?cid=7c7de202e4df4600b614ed6890bf4cba",
      "track_number" : 2,
      "type" : "track",
      "uri" : "spotify:track:5iFwAOB2TFkPJk8sMlxP8g"
    }
  } ],
  "limit" : 1,
  "next" : "https://api.spotify.com/v1/me/tracks?offset=1&limit=1&market=BR",
  "offset" : 0,
  "previous" : null,
  "total" : 333
}
~~~

