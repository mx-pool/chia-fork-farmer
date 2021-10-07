# super-farmer

Super-Farmer是mxpool.org推出的Chia及Chia分叉币多挖程序。只需要运行一个程序，就可以同时挖10个收益最高的分叉币。

程序绿色轻量，压缩后只有6M。

## 安装使用
 * [SuperFarmer 安装使用](https://github.com/mx-pool/super-farmer/wiki/SuperFarmer-%E5%AE%89%E8%A3%85%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97)
 
## 账号注册 & 后台使用
 * 打开 https://mxpool.org 进行账号注册
 * 登录 https://mxpool.org/login
 * 打开用户中心页面 https://mxpool.org/uc/assets 

## 常见问题
 * SuperFarmer是如何工作的?
 
 SuperFarmer是一个兼容Chia协议的客户端，工作原理和chia基本一样。工作过程: 接收网络中的challenge, 在图(plot)文件中寻找证明(proof of space), 找到合适的证明后提交到full_node。区别在于SuperFarmer同时连接到多个分叉网络，同时接收各个网络中的challenge，并提交证明。还有一个区别在于superfarmer不需要本地运行full_node，启动后可立即开始耕种。
 * SuperFarmer是否会使用密钥，是否泄露密钥?
 
 SuperFarmer和官方的chia以相同的方式使用密钥，耕种过程中只会使用farmer key和pool key，用来签名证明(ProofOfSpace)。助记符/farmer key/pool key等私钥均不会上传到网络，只有公钥和签名是会上传到网络。
 * 如何确保钱包密钥安全?
 
 为确保钱包密钥的安全，建议P图/耕种的密钥和钱包的密钥分开。即在一台非耕种的机器上创建一个新的钱包助记符,和耕种使用不同的密钥。

