# Module_2

## 9.Pārbaudīt kāds commit hash ir lokālajā git repozitorijā un salīdzināt to ar šī paša faila commit hash github

README.md faila commit hash:

| Local | Github |
| ------ | ------ |
| d032ae1bc24369985ad14027a9f484e0500084ba | d032ae1bc24369985ad14027a9f484e0500084ba |

## 13.Salīdzināt vienādu failu (ne README) hash no mapes module_1 un module_2. Vai git redz atšķirību starp šiem failiem?

| File | Module1 Hash | Module2 Hash |
| ------ | ------ | ------ |
| git.png | 8138c15badfee809434142735617d02deb014927 | 8138c15badfee809434142735617d02deb014927 |
| task.png | 7056950ff60642fe1efecda44e341a750c9e4db8 | 7056950ff60642fe1efecda44e341a750c9e4db8 |

> Failu hash ir vienadi starp mapem

## 16. Pārbaudīt kādas izmaiņas tika veiktas iepriekšējās nedēļas laikā. Atrast vismaz divus veidus kā to izdarīt.

1.Pievienojot adreses lauka filtru: `?since=2022-05-16` (https://github.com/hashicorp/terraform/commits/main?since=2022-05-16)

2.`git log --since=1.weeks`

## 17. Atrast commit kurus veica autors - “Laura Pacilio”

`git log --author="Laura Pacilio"`

## 18. Atrast vai Laura ir veikusi commit pagājušā gada septembrī?

`git log --author="Laura Pacilio" --after="2021-09-01" --before="2021-09-30"`

## 19. Vai Laura ir veikusi commit vakar?

`git log --author="Laura Pacilio" --since="1 day ago"` vai `git log --author="Laura Pacilio" --since=1.day`
