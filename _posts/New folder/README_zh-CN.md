# Jekyll Theme Chirpy

[![Build Status](https://github.com/cotes2020/jekyll-theme-chirpy/workflows/build/badge.svg?event=push)](https://github.com/cotes2020/jekyll-theme-chirpy/actions?query=event%3Apush)
[![GitHub license](https://img.shields.io/github/license/cotes2020/jekyll-theme-chirpy.svg)](https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/LICENSE)
[![996.icu](https://img.shields.io/badge/link-996.icu-%23FF4D5B.svg)](https://996.icu)

Language: [English](../README.md) | ??����

��?����?�� Jekyll �?��?ݾ����������������??��??��۰��??��η�⡢����?���?��??��

**������?**

* �?���ټ��
* ��������������Ѣ
* ������?
* �?��?��?����
* ?������
* �?��?
* ���
* Atom ??
*  Disqus ??
* Google ���
* GA ???ͱ����?������
* SEO ?��
* ?������?��

[**�???** ��](https://chirpy.cotes.info)

![devices-mockup](https://raw.githubusercontent.com/cotes2020/jekyll-theme-chirpy/master/assets/img/sample/devices-mockup.png)

## ��?

* [��?](#��?)
* [?�����](#?�����)
* [????](#????)
* [��?](#��?)
* [?�](#?�)
* [?ʦ??](#?ʦ??)

## ��?

### ��?����

���� [Jekyll ί۰��?](https://jekyllrb.com/docs/installation/) ������??������? (Ruby��RubyGem��Bundler �� Jekyll)��?������?��?��?���������������??�����? [Python](https://www.python.org/downloads/)( >= 3.5) �� [ruamel.yaml](https://pypi.org/project/ruamel.yaml/)��

����?������ͧ?�� Debian ��� macOS��?���?����?�� [GNU coreutils](https://www.gnu.org/software/coreutils/)����?����?���۰��?��

* Debian

 ```console
 $ sudo apt-get install coreutils
 ```

* macOS

 ```console
 $ brew install coreutils
 ```

��󷣬[fork](https://github.com/cotes2020/jekyll-theme-chirpy/fork) ��?��?������к��? Fork ��??���������߾��

```console
$ git clone git@github.com:USER/jekyll-theme-chirpy.git
```

`USER` ��???�� GitHub username��



### ��? Jekyll ?��

�����?��?��:

```terminal
$ bundle install
```
`bundle` ٤ֵ?�?��? `Gemfile` ??٥����??��.



## ?�����

### ������?

����������������?��

```sh
jekyll-theme-chirpy/
������ _data
������ _includes      
������ _layouts
������ _posts          # posts stay here
������ _scripts
������ .travis.yml     # remove it
������ .github         # remove this, too
������ assets      
������ tabs
��   ������ about.md    # the ABOUT page
������ .gitignore
������ 404.html
������ Gemfile
������ LICENSE
������ README.md
������ _config.yml     # configuration file
������ tools           # script tools
������ docs
������ feed.xml
������ index.html
������ robots.txt
������ sitemap.xml
```


?���?�����������??�:

- .travis.yml
- .github


### ��������

����?����������� `_config.yml` ��?�ᣬ��ݻ��Դ���?˿?������

* ?��
    
    ������?������ۯ���`/assets/img/sample/avatar.jpg`. ��??��?�����?������?�����ң����������(???��??ʦ߾???�ף�*<https://tinypng.com/>* ).

* ??

    ??� `timezone` ��?����?? `?�/߾��`���������??�?���ʦ��֪��?�� [TimezoneConverter](http://www.timezoneconverter.com/cgi-bin/findzone/findzone) ��� [Wikipedia](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).


###  ���?��

�����������ʦ?��?��:

```terminal
$ bash tools/run.sh
```

??�����?�� <http://localhost:4000>

����?��������??�����������������������??���棬ʦ����?? `-r` (�� `--realtime`)����?����?��? [**fswatch**](http://emcrisostomo.github.io/fswatch/) ��

###  ݻ���� GitHub Pages

ݻ��?�����  `_config.yml` �� `url` ��? `https://<username>.github.io`(���?�������٣������`https://yourdomain.com`)��?�⣬����?������ [Project ?��?��](https://help.github.com/en/github/working-with-github-pages/about-github-pages#types-of-github-pages-sites)���������������� `baseurl` ??��٣?�����???������`/project`��

#### ۰�� 1: � GitHub Pages ��������

������۰����?ʦ��������?������?Ӯ??��

> **�**: ����?�������������??[֪��](https://pages.github.com/versions/)߾��?�죬��?�۰���������� [*۰�� 2: ���?��*](#۰��-2-���?��).

**1**. ??��٣?:

|����?�� | ??٣?|
|:---|:---|
|User or Organization | `<username>.github.io`|
|Project| `<username>.github.io` �����٣��ާ�� `project`|

**2**. ���������ǣ�����?��:

```console
$ bash tools/init.sh
```

>**�**: *��������* ֪������������ git ����??��������?������� `_posts` ��?��������ߡ�

??�?���������� *����������Ѣ* �� *��? / ??* ?��.

**3**. ������ `origin/master` ������ GitHub ?????��?? Pages ��?��

**4**. ?��??���

|����?�� | ?�� URL |
|:---|:---|
|User or Organization | `https://<username>.github.io/`|
|Project| `https://<username>.github.io/project/`|


#### ۰�� 2: ���?��

���������ף�GitHub Pages ����?�߲۰?��?��������?������??��������?������?黡�

**1**. �� GitHub ??��?����?����??���������??٤٣: 

|����?�� | ??٣?|
|:---|:---|
|User or Organization | `<username>.github.io`|
|Project| `<username>.github.io` �����٣�� ���� `project`|

���� Clone ��??����򢡣

**2**. ?������:

```console
$ bash tools/build.sh -d /path/to/local/project/
```
> `project` ?��??٣?��

������??����??� `/path/to/local/project`. ����??���������?������?Ӯ `master` ���.

**3**. ���� GithHub ??��?????? Pages ��?��

**4**. ?��??���:

|����?�� | ���� URL |
|:---|:---|
|User or Organization | `https://<username>.github.io/`|
|Project| `https://<username>.github.io/project/`|


### ��?

����??����ʢ��????��??? [?߾?��](https://chirpy.cotes.info/categories/tutorial/)�� ?���?��[Wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki) �����??����͸?��


## ????

߲���������?��?���?ͱ bug, ?���?��??�ᣬ����������������?����????��[���](.github/CONTRIBUTING.md)��????��

## ��?

??�?��??������ [Jekyll](https://jekyllrb.com/) ��?��[Bootstrap](https://getbootstrap.com/)��[Font Awesome](https://fontawesome.com/) �������������������� (��?������ʦ�?��?����������?����).

:tada:��?���??��???���?��, ��?�� GayHub ID �??[֪��](https://github.com/cotes2020/jekyll-theme-chirpy/graphs/contributors)�� ?��, ���? issues(���ڱ����? PR)����ݣ?����ݣڸ���?��?��,��/???�?ͱ bug��������������??���?���������?����?��



## ?�

����?��???�?���???��?𾣬?��?��?����� [?���?](https://github.com/cotes2020/jekyll-theme-chirpy) ��?��? <kbd>:heart:Sponsor</kbd> ??������?��?ʦ������??����?��??�ȣ����?/ڰ��?𾣩��?����????�����?����??���������???�ͣ�


## ?ʦ??

��?��?깣����� [MIT](https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/LICENSE) ?ʦ��