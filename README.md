# nlopt
安装nlopt

sudo apt-get install ros-melodic-nlopt


NLOPT中有多种可以选择的算法，在头文件里面算法名称的枚举类型为

enum algorithm {  
     GN_DIRECT = 0,  
     GN_DIRECT_L,  
     GN_DIRECT_L_RAND,  
     GN_DIRECT_NOSCAL,    
     GN_DIRECT_L_NOSCAL,  
     GN_DIRECT_L_RAND_NOSCAL,  
     GN_ORIG_DIRECT,  
     GN_ORIG_DIRECT_L,  
     GD_STOGO,  
     GD_STOGO_RAND,  
     LD_LBFGS_NOCEDAL,  
     LD_LBFGS,  
     LN_PRAXIS,
     LD_VAR1,   
     LD_VAR2,  
     LD_TNEWTON,  
     LD_TNEWTON_RESTART,  
     LD_TNEWTON_PRECOND,  
     LD_TNEWTON_PRECOND_RESTART,  
     GN_CRS2_LM,    
     GN_MLSL,  
     GD_MLSL,  
     GN_MLSL_LDS,  
     GD_MLSL_LDS,  
     LD_MMA,  
     LN_COBYLA,  
     LN_NEWUOA,  
     LN_NEWUOA_BOUND,  
     LN_NELDERMEAD,  
     LN_SBPLX,  
     LN_AUGLAG,  
     LD_AUGLAG,  
     LN_AUGLAG_EQ,  
     LD_AUGLAG_EQ,  
     LN_BOBYQA,    
     GN_ISRES,  
     AUGLAG,  
     AUGLAG_EQ,  
     G_MLSL,  
     G_MLSL_LDS,  
     LD_SLSQP,   
     LD_CCSAQ,   
     GN_ESCH,  
     NUM_ALGORITHMS /*不是一种算法 只是算法的数量*/   
  };  
  
  
  命名规律：
G/L代表的就是 全局（global）或者局部（local）优化  
N/D代表的就是 不需导数 或者 需要导数 的优化  

例如 LN_COBYLA 就是用的 COBYLA 算法 ，然后该算法用于局部（L）无需导数（N）的优化  
  

更多使用可以参考这个博客

https://www.guyuehome.com/35169
