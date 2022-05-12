# Wordle Helper

Wordle辅助猜词工具
Wordle Game: https://www.nytimes.com/games/wordle/index.html

基本使用方法：

* 当出现"Please Input"的时候，输入一个5个字母的单词，然后打一个空格或换行，再输入5个数字（中间可以空格也可以不空格）
* 数字代表对应位置字母的提示。0代表“不存在”（灰色），1代表“存在但位置不对”（黄色），2代表“位置正确”（绿色）
* 该程序会产生wordle_solves.txt，该文件中给出剩下的所有可能答案
* 在第二次及以后的输入之前，程序会给出一个建议输入

命令行参数设置：

* -r 关闭推荐功能
* -h 打开困难模式（输入的词必须是剩余可能答案中的词）
* -v 输出详细内容（附带输出wordle_predict.txt，包含了输入每个词的推荐值）
* -n 指定推荐功能的搜索阈值（默认为46），剩余答案数量高于阈值时仅在剩余可能答案内搜索，反之在全部可行词内搜索
* 使用示例：./wordle_helper.exe -h -v -n 50

Powered by PbX
