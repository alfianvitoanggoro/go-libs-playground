# go-libs-playground
Playground of golang library

# 📔 STRUCTURE
<pre>
go-library-exploration/
│
├── README.md               ← Dokumentasi utama repo (daftar library, tujuan, dll)
├── go.work                 ← (opsional) Workspace untuk mengelola banyak module
│
└── [name of library]/      ← Eksplorasi untuk library Cobra
    ├── go.mod              ← Modul Go lokal untuk Cobra
    ├── main.go             ← Contoh implementasi utama
    ├── README.md           ← Penjelasan & catatan khusus Cobra
    ├── internal/           ← (opsional) Struktur package jika ingin modular
    ├── config.yaml         ← (opsional) Contoh file config
    ├── docker-compose.yml  ← (opsional)
    ├── dockerfile          ← (opsional)
    └── .env                ← (opsional) konfigurasi koneksi db
</pre>

# 🎲 SUBMODULE
A submodule lets you keep a separate repository (Repo B) inside the working directory of your main repository (Repo A), while still keeping them versioned independently.

Think of it like this:

- You have Project A

- Inside it, you want to include Library X that lives in a different repo

- Instead of copy-pasting the code, you add Library X as a submodule

## Add submodule repository
<pre>
git submodule add https://github.com/username/repository-name.git repository-name
</pre>

## Pull submodule repository
<pre>
git submodule update --init --recursive repository-name
</pre>

## Update submodule repository
<pre>
git submodule update --remote --merge repository-name
</pre>

## Pull All submodule repository
<pre>
git submodule update --init --recursive
</pre>

## Update All submodule repository
<pre>
git submodule update --remote --merge
</pre>
