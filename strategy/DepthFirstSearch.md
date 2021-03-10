# Depth First Search
This is the strategy for systematically mastering Depth First Search, especially ones related to DP/DFSMemo.

### Phase 1: Binary Tree - DFS
DFS on binary trees are fundamentals and thus important: <br/>
* as good candidates to practice recursion 
    * is it top-down or bottom-up approach?
    * what characterizes the current/next state?
    * how states are passed among different levels of call stacks?
    * does/can the recursion return anything? If yes, what is/are it/they?
    * how about dealing with more than one levels of call stacks at one time?
* as decision trees for later advanced DP/DFSMemo problems

*[Problem List - Abstract](https://github.com/an7one/leetcode-problems-by-tags-an7one/blob/master/txt/by_data_structure/tree/abstract.txt) <br/>
[Problem List - Complete](https://github.com/an7one/leetcode-problems-by-tags-an7one/blob/master/txt/by_data_structure/tree)

| Scores | Description                                                                                                                                                                                                                                   |
| ------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 60%    | to master recursive preorder, inorder, postorder traversals<ul> <li> to construct a binary tree freely</li> <li>to operate on a binary tree freely, including insersion, deletion, etc.</li> <li>to serialize and deserialize tree freely<ul> |
| 80%    | to master iterative preorder, inorder, postorder traversals<ul><li>to simulate recursions with stacks</li><li>Morris inorder traversal, and its variations</li></ul>                                                                          |
| 100%   | to quickly detect and build decision trees (especially for advanced DP problems)                                                                                                                                                              |

### *Must Read/Watch
##### labuladong
东哥手把手带你套框架刷通二叉树|第一期 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247487126&idx=1&sn=4de13e66397bc35970963c5a1330ce18&chksm=9bd7f09eaca0798853c41fba05ad5fa958b31054eba18b69c785ae92f4bd8e4cc7a2179d7838&scene=21#wechat_redirect) <br/>
东哥手把手帮你刷通二叉树|第二期 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247487270&idx=1&sn=2f7ad74aabc88b53d94012ceccbe51be&chksm=9bd7f12eaca078384733168971147866c140496cb257946f8170f05e46d16099f3eef98d39d9&scene=21#wechat_redirect) <br/>
东哥手把手带你刷二叉树|第三期 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247487527&idx=1&sn=9cf2b0d8608ba26ea7c6a5c9b41d05a1&chksm=9bd7ee2faca0673916bf075539bf6fc3c01f3dcc0b298b3f507047692ef5c850ed9cfe82e4e6&scene=21#wechat_redirect) <br/>
手把手刷二叉搜索树（第一期 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247488101&idx=1&sn=6041ddda5f20ccde8a7036d3e3a1482c&chksm=9bd7ec6daca0657b2ab20a936437e2c8206384c3b1485fe91747ad796fa3a5b08556b2f4911e&scene=21#wechat_redirect) <br/>
原创 | 手把手刷二叉搜索树（第二期）[WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247488128&idx=2&sn=b8fb3fd2917f9ac86127054741cd5877&chksm=9bd7ec88aca0659ee0185b657663169169493e9df2063fa4d28b38a0b4d0dd698d0301937898&scene=21#wechat_redirect) <br/>
二叉树的题，就那几个框架，枯燥至极🤔 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247485871&idx=1&sn=bcb24ea8927995b585629a8b9caeed01&chksm=9bd7f7a7aca07eb1b4c330382a4e0b916ef5a82ca48db28908ab16563e28a376b5ca6805bec2&scene=21#wechat_redirect) <br/>
题目不让我做什么，我就偏要去做什么🤔 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247485629&idx=1&sn=fc0d0fc2b8618a9b8a575cfa9d5b1c4a&chksm=9bd7f6b5aca07fa33c4fbce0dc439359592ace091814fdcdc0742f336722398090396f0b3668&scene=21#wechat_redirect) <br/>
用 Git 来讲讲二叉树最近公共祖先 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247485561&idx=1&sn=a394ba978283819da1eb34a256f6915b&chksm=9bd7f671aca07f6722f0bc1e946ca771a0a40fd8173cc1227a7e0eabfe4e2fcc57b9ba464547&scene=21#wechat_redirect) <br/>
完全二叉树的节点数，你真的会算吗 [WeChat](https://mp.weixin.qq.com/s?__biz=MzAxODQxMDM0Mw==&mid=2247485057&idx=1&sn=45a3b89a4efef236cb662d5505d7ce36&chksm=9bd7f889aca0719f4915de681f983355e187151030991ab1944494ffe4b73e484068b85eb01e&scene=21#wechat_redirect) <br/>

##### HuaHua
LeetCode Binary Trees 二叉树 - 刷题找工作 SP12 [Youtube](https://youtu.be/PbGl8_-bZxI)

##### 大雪菜
LeetCode暑期刷题打卡2019——Week3 树专题 [Bilibili](https://www.bilibili.com/video/BV19t411w7Ep)

##### OTTFF
[[Algorithm][007] 深度优先搜索 Depth First Search (DFS)](https://www.bilibili.com/video/BV1z4411278H)


****
### Phase 2: DFS with Memoization
Main Track: **DFS with Memoization** <br/>
Actually on decision trees.

(Not yet finished) *[Problem List - Abstract](https://github.com/An7One/leetcode-problems-by-tags-an7one/blob/master/txt/by_algorithm/search/depth_first_search/abstract.txt) <br/>
[Problem List - Complete](https://github.com/An7One/leetcode-problems-by-tags-an7one/blob/master/txt/by_algorithm/search/depth_first_search/by_algorithm/dfs_with_memoization.txt)

Secondary Track: <br/>
[Backtrack](https://github.com/An7One/leetcode-problems-by-tags-an7one/blob/master/txt/by_algorithm/search/depth_first_search/by_algorithm/backtrack.txt) <br/>
[DFS on Undirected Graph](https://github.com/An7One/leetcode-problems-by-tags-an7one/blob/master/txt/by_algorithm/search/depth_first_search/by_data_structure/graph/graph_undirected.txt) <br/>
[DFS on Directed Graph](https://github.com/An7One/leetcode-problems-by-tags-an7one/blob/master/txt/by_algorithm/search/depth_first_search/by_data_structure/graph/graph_directed.txt) <br/>
[DFS on String](https://github.com/An7One/leetcode-problems-by-tags-an7one/tree/master/txt/by_algorithm/search/depth_first_search/by_data_structure/string) <br/>
[DFS on Array](https://github.com/An7One/leetcode-problems-by-tags-an7one/tree/master/txt/by_algorithm/search/depth_first_search/by_data_structure/array) <br/>

### Phase 3: Dynamic Programming
Actually on decision trees. <br/>
To be continued...