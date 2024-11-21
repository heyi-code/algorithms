<font style="color:rgb(38, 38, 38);background-color:rgb(240, 240, 240);">Trie 是一颗非典型的</font>**<font style="color:rgb(38, 38, 38);background-color:rgb(240, 240, 240);">多叉树模型</font>**<font style="color:rgb(38, 38, 38);background-color:rgb(240, 240, 240);">，多叉好理解，即每个结点的分支数量可能为多个。</font>

<font style="color:rgb(38, 38, 38);background-color:rgb(240, 240, 240);"></font>

```java
class TrieNode {
    private boolean isEnd;  // 标记该节点是否为某个单词的结尾
    private TrieNode[] next;    // 后续节点数组

    TrieNode() {
        isEnd = false;
        next = new TrieNode[26];
    }
}
```

<font style="color:rgb(38, 38, 38);background-color:rgb(240, 240, 240);"></font>

<font style="color:rgb(38, 38, 38);background-color:rgb(240, 240, 240);">包含三个单词 "sea","sells","she" 的 Trie，如下所示，并不直接保存字符本身，而是通过下标的映射关系确定。</font>

![](https://cdn.nlark.com/yuque/0/2024/png/50802488/1732176919986-1d3612fd-ca7a-4db1-98df-504814f0d564.png)

详解：[https://leetcode.cn/problems/implement-trie-prefix-tree/solutions/98390/trie-tree-de-shi-xian-gua-he-chu-xue-zhe-by-huwt](https://leetcode.cn/problems/implement-trie-prefix-tree/solutions/98390/trie-tree-de-shi-xian-gua-he-chu-xue-zhe-by-huwt)

