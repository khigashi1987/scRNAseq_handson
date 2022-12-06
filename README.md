# scRNAseq_handson
PythonによるシングルセルRNA-seq解析。

### 前半

1. Scanpy (前処理)
2. scVI (深層生成モデルによるバッチ補正とデノイジング)

[HTML資料へのリンク](https://khigashi1987.github.io/scRNAseq_handson/Python_scRNAseq_1.html)

[Google Colaboratoryバージョンの資料へのリンク]()

### 後半

3. CellAssign (Cell typeの自動推定)
4. scANVI (アトラスとの統合とラベル転移)
5. scVelo (RNA速度)
6. CellRank (Trajectory解析)

[HTML資料へのリンク](https://khigashi1987.github.io/scRNAseq_handson/Python_scRNAseq_2.html)

[Google Colaboratoryバージョンの資料へのリンク]()

## Dockerで実行する場合

```bash
docker pull koichihigashi/pags_bioinfo2022:v2
git clone https://github.com/khigashi1987/scRNAseq_handson.git
cd scRNAseq_handson
docker run \
    -p 8888:8888 \
    -v $(PWD):/work/scRNAseq_handson \
    pags_bioinfo2022:v2
```
出力されたリンク（http://127.0.0.1:8888/...のほう）をブラウザで開く。