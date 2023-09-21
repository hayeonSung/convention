# 🙏 Commit Rule

### 메시지 구조

```
[Type] Subject
--blank line-- 
Body (optional)
--blank line--
Footer(optional)
```

```
$ git commit -m "this is Subject
>> 
>> this is Body
>> 
>> this is Footer"
 
// Summary(required) 란에 Type: Subject 입력
// Description 란에 Body와 Footer입력 
```

<br />

### Type

※ Type 첫 문자는 대문자 (CI 예외)

| Commit Type | Description                                                  |
| ----------- | ------------------------------------------------------------ |
| Feat        | 새로운 기능, 코드 추가                                       |
| Fix         | 올바르지 않은 동작(버그) 수정                                |
| Update      | 개정, 개선, 버전 업데이트, API 변동                          |
| Remove      | 코드 삭제. ‘unnecessary’, ‘useless’, ‘unused’ 등의 수식어 활용 |
| Docs        | 문서 수정 (Readme 등)                                        |
| Comment     | 필요한 주석 추가 및 변경                                     |
| Refactor    | 코드 리팩토링                                                |
| Design      | CSS, Image 등 사용자 UI 디자인 변경                          |
| Style       | 코드 스타일 혹은 포맷 수정                                   |
| Build       | 빌드 관련 파일 수정                                          |
| CI          | CI 관련 설정 변경                                            |
| Chore       | 그 외 자잘한 수정                                            |

<br />

### Subject, Body, Footer

| Message Part | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| Subject      | 영어/한글 최대 50글자. 마침표 및 특수기호 사용 X 첫글자는 대문자로 작성 현재 시제 사용 [ Changing, Changed (x) -> Change (o) ] 부연 설명 필요시 Body 활용 |
| Body         | 한 줄당 72자 내 작성. 필요시 개행 '무엇을', '어떻게', '왜' 변경했는지 작성 필수 가능한 상세히 작성(optional) |
| Footer       | Footer은 optional 참고할 이슈번호 기재 Ref: #이슈번호 ex) Ref: #34, #23 (optional)|

<br />

# 📜 Branch Rule

### 과정

**develop** 의 최신 commit에서 각자 작업 브랜치 생성

작업 수행 후 commit하여 develop branch에 pull request

Merge시, squash-merge로 진행

하나의 브랜치당 하나의 커밋을 유지 (force-push)

<br />

### 브랜치 명

| Branch Level | Description                            |
| ------------ | -------------------------------------- |
| main (m)     | 최종 확인 완료                         |
| hotfix (h)   | 최종 배포 버전에서의 오류 긴급 수정    |
| develop (d)  | 기능 개발 및 수정, 오류 해결 완료 버전 |
| feature (f)  | 각자 작업                              |

| Work Category | Description                                     |
| ------------- | ----------------------------------------------- |
| new           | 새로운 기능, 코드 추가                          |
| fix           | fix, update, refactor, remove 등 기능 개선 일체 |


# 테스트
- WIP
