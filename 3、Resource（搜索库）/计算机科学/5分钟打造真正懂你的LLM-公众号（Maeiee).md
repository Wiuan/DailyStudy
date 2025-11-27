[[3、Resource（搜索库）/工作流配置（配置、插件、网页、Prompt）/prompt]]
```
#!/bin/bash  
  
# know_my_self.sh - 生成用于训练 LLM 的 Prompt，包含 Maeiee 的个人信息  
  
# 检查 README.md 文件是否存在  
if [ ! -f "README.md" ]; then  
    echo "错误: README.md 文件不存在"  
    exit 1  
fi  
  
# 定义输出文件  
OUTPUT_FILE="know_my_self.txt"  
  
# 生成 Prompt 并保存到文件  
{  
cat << 'EOF'  
我是 Maeiee，我准备训练一个 LLM，我想训练一个懂我的 LLM，因此我正在编写一个介绍我自己的数据集。但是我发现凭空往上写很吃力，要是有人向我提问，我回答问题会容易得多。  
  
因此，我想请你担任《Maeiee 数据集》的提问者，我向你发送数据集的全部内容，你问我20个问题，问题的答案就是数据集的新增内容，用于介绍我自己的方方面面。  
  
关于问题的范围，不仅限于我数据集中的已有问题，只要是用于介绍我自己的任何问题都可以，也可以包含隐私问题。  
  
你只需向我不断提出问题即可。我会自己往数据集中添加回答，在所有对话中，你只管提问。  
  
<Maeiee 数据集>  
EOF  
  
# 插入 README.md 的内容  
cat README.md  
  
cat << 'EOF'  
</Maeiee 数据集>  
EOF  
} > "$OUTPUT_FILE"  
  
echo "Prompt 已生成并保存到 $OUTPUT_FILE"
```