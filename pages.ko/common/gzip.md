# gzip

> `gzip` 압축 (LZ77)을 사용하여 파일 압축/압축 해제.
> 더 많은 정보: <https://www.gnu.org/software/gzip/manual/gzip.html>.

- 파일을 압축하여, `gzip` 아카이브로 대체:

`gzip {{경로/대상/파일}}`

- 파일의 압축을 풀어, 원래의 압축되지 않은 버전으로 교체:

`gzip {{[-d|--decompress]}} {{경로/대상/파일.gz}}`

- 원본 파일을 유지하면서, 파일을 압축:

`gzip {{[-k|--keep]}} {{경로/대상/파일}}`

- 출력 파일 이름을 지정하여, 파일을 압축:

`gzip {{[-c|--stdout]}} {{경로/대상/파일}} > {{경로/대상/압축된_파일.gz}}`

- 출력 파일 이름을 지정하여, `gzip` 아카이브의 압축을 품:

`gzip {{[-c|--stdout]}} {{[-d|--decompress]}} {{경로/대상/파일.gz}} > {{경로/대상/압축해제된_파일}}`

- 압축 수준을 지정. 1은 가장 빠르며 (낮은 압축), 9는 가장 느림 (높은 압축), 6은 기본값:

`gzip -{{1..9}} {{[-c|--stdout]}} {{경로/대상/파일}} > {{경로/대상/압축된_파일.gz}}`

- 압축 또는 압축 해제된 각 파일의 이름과 감소 비율을 표시:

`gzip {{[-v|--verbose]}} {{[-d|--decompress]}} {{경로/대상/파일.gz}}`
