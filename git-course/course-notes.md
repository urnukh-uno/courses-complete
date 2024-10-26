# Git, Github эхнээс нь дуустал!

## Table of Contents

- [Install Git](#install-git)
- [Delete Git](#delete-git)
- [Setup Remote Git](#setup-remote-git)\
- [Git Lifecycle](#git-lifecycle)

<br>

### Common Git Commands

|     | Git коммандууд                     | Тайлбар                                                                     |
| :-: | :--------------------------------- | :-------------------------------------------------------------------------- |
|  1  | brew install git                   | Homebrew буюу package manager ашиглан Git татаж суулгана                    |
|  2  | git init                           | .Git file -ийг төсөл дотроо үүсгэнэ                                         |
|  3  | git status                         | Төслийн өөрчлөлтийг track хийнэ                                             |
|  4  | ls -lah                            | Төсөлтэй холбоотой Git -ийн тохиргоог шалгана                               |
|  5  | rm -rf .git                        | Төсөл дотор үүсгэсэн .Git file болон түүний тохиргоо тэр чигтэй устна       |
|  6  | git remote -v                      | Локал төсөл маань remote repository линктэй холбогдсоныг шалгаж харуулна    |
|  7  | git remote add origin [HTTPS линк] | Локал төсөлтэй remote repository линкийг холбоно                            |
|  8  | git add -A                         | Төсөл дээр хийгдсэн бүх шинэчлэлтийг локал git дээр нэмнэ                   |
|  9  | git commit -m "тайлбар"            | Локал git дээр нэмсэн бүх өөрчлөлтийг өөрчлөлт болгож баталгаажуулна        |
| 10  | git push origin master             | Локал git дээр баталгаажсан бүх өөрчлөлтийг Github repo -той merge хийнэ    |
| 11  | git checkout -- .                  | Локал git дээр хамгийн сүүлд байсан хувилбарын дагуу бүх файлуудыг сэргээнэ |

<br>

#### Install Git

`2024.10.16`

Homebrew буюу package manager ашиглан Git татаж суулгах ба Git файлыг төсөл дотроо үүсгэж, үүсгэсэн эсэхээ шалгаж сурна.

> [!NOTE]
>
> - Эхлээд [Link](https://git-scm.com/downloads/mac) -рүү орно. `$ brew install git` script -ийг уншуулж brew суулгана.
> - Track хийхийг хүссэн төслийн файл дотроо `$ git init` script -ийг уншуулж git файл үүсгэнэ.
> - `$ git status` script -ийг уншуулж одоогийн файлуудын статусыг шалгана.
> - `$ ls -lah` script -ийг уншуулж нуугдсан .git folder үүссэн эсэхийг шалгана.

[Go top](#table-of-contents)

<br>

#### Delete Git

`2024.10.17`

Local ажиллуулж буй төсөл дотор үүссэн .Git файлыг хадгалсан түүх болон тохигооных нь хамт тэр чигт нь устгаж сурна.

> [!NOTE]
>
> - `$ rm -rf .git` script -ийг уншуулснаар төсөл дотор үүсгэсэн .Git file болон түүний тохиргоо тэр чигтэй устна.

[Go top](#table-of-contents)
<br>

#### Setup Remote Git

`2024.10.18`

Local дээр үүсгэсэн файлуудаа Github -тай холбож сурна.

> [!NOTE]
>
> - Github аккаунт үүсгэнэ.
> - Github аккаунт дотроо шинэ repository үүсгэнэ.
> - Үүсгэсэн repository -ийн "<> Code" товчлуур дээр дарахаар HTTPS линк гарч ирэх ба түүнийг хуулж авна.
> - `$ git remote -v` script -ийг уншуулж Github -руу хуулах төсөл нь өөр remote repository -той холбогдоогүй эсэхийг заавал шалгана.
> - `$ git remote add origin [HTTPS линк]` script -ийг уншуулж локал дотор төслөө Github repository -тойгоо холбож өгнө.
> - `$ git remote -v` script -ийг уншуулж холбогдсон эсэхийг шалгана. Холбогдсон тохиолдолд холбосон линк гарч ирэх ётой.
> - `$ git add -A` , `$ git commit -m "Тайлбар"` , `$ git push origin master"` script -ийг уншуулж Github -руугаа локал төслийнхөө файлыг хуулна.

[Go top](#table-of-contents)

<br>

#### Git Lifecycle

`2024.10.26` `Хичээл-14`
Git файлуудын амьдарлын цикл (untracked, modifed, staged, unmodified), устгагдсан төслийг сэргээх, git log түүх харах
Git file -ууд үүсэхээс авхуулаад устах хүртэлх амьдралын цикл буюу статусууд

> [!NOTE] **Git -ийн статусууд**
>
> - Untracked (Бүртгэлгүй)
>   - Unmodified төлвийн файлыг буцааж бүртгэлгүй болговол энэ төлөвт шилждэг
> - Modified (Өөрчлөгдсөн)
>   - Unmodified төлөвтэй байсан файлыг өөрчилж, устгавал энэ төлөвт шилждэг
> - Staged (Сонгогдсон)
>   - Untracked эсвэл Modified төлвөөс `git add` комманд өгч уг төлөврүү шилжинэ
> - Unmodified (Өөрчлөлтгүй)
>   - Staged төлвөөс `git commit` комманд өгч уг төлөвт шилжинэ

> [!NOTE]
>
> - `$ git checkout -- .` script -ийг уншуулж хамгийн сүүлд байсан хувилбарын дагуу бүх файлуудыг сэргээнэ.

[Go top](#table-of-contents)
<br>
