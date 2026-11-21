# permission

Data whitelist IP untuk autoscript [`Masbrow33/btr`](https://github.com/Masbrow33/btr).

Dipakai oleh `update/menu-ip.sh`:

```
curl -sS https://raw.githubusercontent.com/<username>/permission/main/ipmini
```

## Format `ipmini`

```
### <client> <exp> <ip> <admin>
```

- kolom 4 = IP
- kolom 5 = `ON` (aktif) / `OFF` (diblokir)

## Setup

Di VPS, isi dulu identitas git lewat menu IP:

```
/etc/yokkovpn/github/username   -> username GitHub kamu
/etc/yokkovpn/github/email      -> email GitHub
/etc/yokkovpn/github/api        -> personal access token (scope repo)
```

Script akan clone repo ini, menambahkan entri, lalu push kembali.
