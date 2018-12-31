# 区块链期末项目捐款系统



---

## 选题背景
慈善捐款越来越普遍，但该行业仍然存在着多年运作累积的很多问题。最令人诟病的就是善款去向不明、信息不公开，而且公益项目，每一笔善款都代表着公众对需要帮助的人的爱心和善意，一旦曝出贪污等不法行为，打击几乎是毁灭性的。在某些特定的情况下，这些问题也阻碍了人们奉献爱心。而区块链的出现正好为慈善捐款的公平公正提供了基础。


## 依据
区块链技术具有数据不可篡改和可追溯性，可以用来构建监管部门所需要的，包含众多手段的监管工具箱。以利于实施精准、及时和更多纬度的监管。利用区块链来实现一个基金会的捐款系统，可以准确记录用户的每一笔捐款，明确每一次捐款的细则，避免了一些伪造的捐款、夸大数额的捐款出现。区块链在慈善领域有以下多个优势：

1. 降低交易成本 
区块链上的交易是可以点对点完成的，你可以直接将钱捐赠给指定的人或机构，无须转手多家银行和机构，这将有效减少交易成本。
2. 增加透明度
 区块链技术可以使捐赠的环节更加透明，每一次捐赠都会直接记录在分布式账本数据库中，记录公开透明可查询且不可篡改，当然，你也可以通过账本追溯捐款的去向。
3. 增强信任
  区块链技术可以使人们快速建立信任关系，消除了捐助者对第三方的需求，这意味着2.0版的慈善机构和非营利性机构将不再依靠其他机构，如银行、律师和政府实体等。

## 使用说明
### 一、安装Node
在[官方网址][1]下载安装包，选择LTSQ版本下载。

![此处输入图片的描述][2]

安装后在windows命令cmd窗口，输入node -v，能显示node的版本就成功第一步了

### 二、安装Truffle
truffle是本地的用来编译、部署智能合约的工具。
在windows命令行窗口输入npm -g install truffle。

安装完成后输入truffle，检测truffle是否被正确安装
![此处输入图片的描述][3]

### 三、安装以太坊客户端
智能合约必须要部署到链上进行测试。可以选择部署到一些公共的测试链比如Rinkeby或者Ropsten上，缺点是部署和测试时间比较长，而且需要花费一定的时间赚取假代币防止out of gas。
这里使用了Ganache客户端，并且是带有图形界面的版本。
[下载地址][4]
打开Ganache，进入图形界面
![此处输入图片的描述][5]

选择QUICKSTART，Ganache默认建立十个用户，每个用户有100ETH的余额。
![此处输入图片的描述][6]
Ganache默认运行在7545端口，可以在界面右上方的“设置”里进行更改。

### 四、编译合约
输入truffle compile编译合约
![此处输入图片的描述][7]
### 五、部署合约
输入truffle migrate部署合约
![此处输入图片的描述][8]


### 六、启动服务
输入命令npm run dev
![此处输入图片的描述][9]

使用webpack可以实时编译界面改动

### 测试
进入应用主界面
![此处输入图片的描述][10]
直接点击捐献目标
![此处输入图片的描述][11]

添加捐献目标
![此处输入图片的描述][12]

为序号1的目标捐赠10eth
![此处输入图片的描述][13]

给不存在的目标捐款
![此处输入图片的描述][14]
转账金额超出账户余额（默认余额为100eth）
![此处输入图片的描述][15]

捐赠细则
![此处输入图片的描述][16]

交易返回值
![此处输入图片的描述][17]

## Github源码链接
[https://github.com/stwie2k/Blockchain_finalproject][18]


  [1]: https://nodejs.org/en/
  [2]: https://i.loli.net/2018/12/29/5c271cd9b3e29.png
  [3]: https://i.loli.net/2018/12/29/5c273c00cda2a.png
  [4]: https://github.com/trufflesuite/ganache/releases
  [5]: https://i.loli.net/2018/12/29/5c273c261a071.png
  [6]: https://i.loli.net/2018/12/29/5c273c852c29d.png
  [7]: https://i.loli.net/2018/12/30/5c28e36d3ccff.png
  [8]: https://i.loli.net/2018/12/31/5c28f531eeded.png
  [9]: https://i.loli.net/2018/12/31/5c28f55ecd62b.png
  [10]: https://i.loli.net/2018/12/31/5c28f753eee62.png
  [11]: https://i.loli.net/2018/12/31/5c29b52cb12e9.png
  [12]: https://i.loli.net/2018/12/31/5c29a6d429aa4.png
  [13]: https://i.loli.net/2018/12/31/5c29aa7e5197d.png
  [14]: https://i.loli.net/2018/12/31/5c29b5d52428b.png
  [15]: https://i.loli.net/2018/12/31/5c29f8c5758e9.png
  [16]: https://i.loli.net/2018/12/31/5c29aa93c94c9.png
  [17]: https://i.loli.net/2018/12/31/5c29aacaefa0d.png
  [18]: https://github.com/stwie2k/Blockchain_finalproject
