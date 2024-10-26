# Git, Github эхнээс нь дуустал!

## Table Of Contents

- [Install Git](#install-git)
- [Delete Git](#delete-git)

<br>

### Common Git Commands

|  | Git коммандууд | Тайлбар |
| :-: | :- | :- |
| 1 | brew install git | Homebrew буюу package manager ашиглан Git татаж суулгана |
| 2 | git init | .Git file -ийг төсөл дотроо үүсгэнэ |
| 3 | git status | Төслийн өөрчлөлтийг track хийнэ |
| 4 | ls -lah | Төсөлтэй холбоотой Git -ийн тохиргоог шалгана |

<br>

#### Install Git

`2024.10.16`

Homebrew буюу package manager ашиглан Git татаж суулгах ба Git файлыг төсөл дотроо үүсгэж, үүсгэсэн эсэхээ шалгаж сурна.

> [!NOTE]
> Эхлээд [Link](https://git-scm.com/downloads/mac) -рүү орно. `$ brew install git` script -ийг уншуулж brew суулгана.
> Track хийхийг хүссэн төслийн файл дотроо `$ git init` script -ийг уншуулж git файл үүсгэнэ.
> `$ git status` script -ийг уншуулж одоогийн файлуудын статусыг шалгана.
> `$ ls -lah` script -ийг уншуулж нуугдсан .git folder үүссэн эсэхийг шалгана.

[Go top](#common-git-commands)

<br>

#### Delete Git

`2024.10.17`

Local ажиллуулж буй төсөл дотор үүссэн .Git файлыг хадгалсан түүх болон тохигооных нь хамт тэр чигт нь устгаж сурна.

> [!NOTE]
> `$ rm -rf .git` script -ийг уншуулснаар төсөл дотор үүсгэсэн .Git file болон түүний тохиргоо тэр чигтэй устна.

[Go top](#common-git-commands)
<br>
