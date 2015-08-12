#friso词库结构和管理.

# friso词库结构 #

friso的词库分词八类：

```
#friso lexicon configure file.
# @email	chenxin619315@gmail.com
# @date		2012-12-19
#main lexion
__LEX_CJK_WORDS__ :[
	lex-main.lex;
	lex-admin.lex;
	lex-chars.lex;
	lex-cn-mz.lex;
	lex-cn-place.lex;
	lex-company.lex;
	lex-festival.lex;
	lex-flname.lex;
	lex-food.lex;
	lex-lang.lex;
	lex-nation.lex;
	lex-net.lex;
	lex-org.lex;
#add more here
]
#single chinese unit lexicon
__LEX_CJK_UNITS__ :[
	lex-units.lex;
]
#chinese and english mixed word lexicon.
__LEX_MIX_WORDS__:[
	lex-mixed.lex;
]
#chinese last name lexicon.
__LEX_CN_LNAME__:[
	lex-lname.lex;
]
#single name words lexicon.
__LEX_CN_SNAME__:[
	lex-sname.lex;
]
#first word of a double chinese name.
__LEX_CN_DNAME1__:[
	lex-dname-1.lex;
]
#second word of a double chinese name.
__LEX_CN_DNAME2__:[
	lex-dname-2.lex;
]
#chinese last name decorate word.
__LEX_CN_LNA__:[
	lex-lna.lex;
]

```

每个词条占一行。
含义如下：

词条/词性/同义词(多个使用,隔开)

例如：(值不确定请使用null代替)

高性能/null/优质

### 如何给friso新建词库 ###

1.在friso的词库文件夹下建立一个以utf-8编码的文本文件（命名不限）。
为了统一，建议以lex-开头和.lex作为后缀。

2.在friso.lex.ini中加入新建的词库：

依据的你的词库的分类，把词库文件名加入到friso.lex.ini中即可。

### 如何给已有的词库加入新词条 ###
找到对应的词库文件，使用文本编辑器打开。

按照：“词条/词性/同义词列表” 的格式加入词条作为一行即可。