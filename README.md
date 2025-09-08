SMAC (StarCraft Multi-Agent Challenge) 是一个强化学习平台，专门用于研究星际争霸游戏中的多智能体行为。SMAC 平台是一个使用 PySC2 游戏引擎构建的仿真环境，可以让研究人员在其中开展多种强化学习算法的实验。
配置环境：
1. 下载SMAC地图（Releases · oxwhirl/smac (github.com)），解压放进安装好的星际争霸StarCraft II文件下面的Maps目录中（压缩包中已下好）：

2. 安装PySC2以及安装SMAC（oxwhirl/smac: SMAC: The StarCraft Multi-Agent Challenge (github.com)）：
pip install pysc2
pip install git+https://github.com/oxwhirl/smac.git
（我第二步网络不好会卡顿，选择先克隆再安装）：
git clone https://github.com/oxwhirl/smac.git
pip install -e smac/
 
注意：pip要升级到最新，否则可能会报错：
pip-install--upgrade-pip

3. 测试地图是否正确读出：
python -m smac.bin.map_list

4. 测试SMAC及其映射是否正确安装（要稍微多等一会）：
python -m smac.examples.random_agents

相关参考：
SMAC——星际争霸多智能体实验环境 - 知乎 (zhihu.com)
星际争霸2 -- SMAC 环境介绍 - 知乎 (zhihu.com)
多智能体强化学习环境【星际争霸II】SMAC环境配置_二向箔不会思考的博客-CSDN博客
smac/smac.md at master · oxwhirl/smac (github.com)
