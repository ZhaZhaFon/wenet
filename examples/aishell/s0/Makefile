stage-1: # 下载AISHELL-1
	bash run.sh --stage -1 --stop-stage -1

stage-0: # 准备数据列表 生成data/
	bash run.sh --stage 0 --stop-stage 0 \
				--data /home/jiangji/basic/corpus/aishell-1

stage-1: # 数据列表处理(去除data/{x}/text里中文transcript的空格) 数据统计(CMVN)
	bash run.sh --stage 1 --stop-stage 1

stage-2: # 准备数据 中字=>token 生成data/dict/lang_char.txt
	bash run.sh --stage 2 --stop-stage 2

stage-3: # 准备数据
	bash run.sh --stage 3 --stop-stage 3