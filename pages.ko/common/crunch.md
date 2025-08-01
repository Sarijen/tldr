# crunch

> 단어 목록 생성기.
> 더 많은 정보: <https://manned.org/crunch>.

- 소문자만 사용하여 길이가 1부터 3인 단어 목록을 출력:

`crunch {{1}} {{3}}`

- 길이가 8인 16진수 단어 목록을 출력:

`crunch {{8}} {{8}} {{0123456789abcdef}}`

- abc의 모든 순열 목록을 출력 (길이는 처리되지 않음):

`crunch {{1}} {{1}} -p {{abc}}`

- 주어진 문자열의 모든 순열 목록을 출력 (길이는 처리되지 않음):

`crunch {{1}} {{1}} -p {{abc}} {{def}} {{ghi}}`

- 주어진 패턴에 따라 생성된 단어 목록과 최대 중복 문자 수를 출력:

`crunch {{5}} {{5}} {{abcde123}} -t {{@@@12}} -d 2@`

- 주어진 문자열로 시작하여 주어진 크기의 청크 파일에 단어 목록을 작성:

`crunch {{3}} {{5}} -o {{START}} -b {{10kb}} -s {{abc}}`

- 주어진 문자열에서 멈추고 단어 목록을 반전시켜 단어 목록을 작성:

`crunch {{1}} {{5}} -o {{START}} -e {{abcde}} -i`

- 지정된 단어 수로 압축된 청크 파일에 단어 목록을 작성:

`crunch {{1}} {{5}} -o {{START}} -c {{1000}} -z {{gzip|bzip2|lzma|7z}}`
