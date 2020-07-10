1. 错误说明：np.load() 缺少allow_pickle的权限
2. 解决途径：在load方法中添加属性(修改allow_pickle为True)；np.load("npz路径", allow_pickle = True) 