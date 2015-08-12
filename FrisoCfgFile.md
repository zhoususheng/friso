#friso.ini配置文件使用说明.

## friso.ini配置文件 ##

```
#friso configuration file.
#	do not change the name of the left key.
# @email	chenxin619315@gmail.com
# @date		2012-12-20
#

#lexicon directory absolute path.
#	the value must end with '/'
#this will tell friso how to find friso.lex.ini configuration file and all the lexicon files.
#词库配置文件friso.lex.ini目录，必须以"/"结尾。
friso.lex_dir = /c/friso/dict/

#the maximum matching length.
#最大切分词长度
friso.max_len = 5

#1 for recognition chinese name.
#	and 0 for closed it.
#是否开启中文姓名识别(1表示开启，0表示关闭)。
friso.r_name = 1

#the maximum length for the cjk words in a
#	chinese and english mixed word.
#重要混合词中中文词的最大长度。
friso.mix_len = 2

#the maxinum length for the chinese last name adron.
#姓氏修饰词的最大长度。（例如：老成中的“老”）
friso.lna_len = 1

#append the synonyms words
#是否自动追加切分同义词
friso.add_syn = 1

#clear the stopwords or not (1 to open it and 0 top close it)
#是否自动过滤停止词
friso.clr_stw = 1

#the threshold value for a char not a part of a chinese name.
#姓名识别歧义厥值。
friso.nthreshold = 2000000

#default mode for friso.
# 1 : simple mode - simply maxmum matching algorithm.
# 2 : complex mode - four rules of mmseg alogrithm.
#分词模式，1->简易模式，2->复杂模式。
friso.mode = 2

```