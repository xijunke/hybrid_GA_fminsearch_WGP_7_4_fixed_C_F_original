# 说明注释区别(Explanation of differences in annotations)

# 由hybrid_GA_fminsearch_wings_morphology_6修改而来，20160106日之前该论文的一些气动力和力矩以及功率的计算程序有小错误

# 目前改程序已经修改，几近正确

0.hybrid_GA_fminsearch_WingM4_4_2由hybrid_GA_fminsearch_WingM4_4_1进化修改而来

1.该文件夹下为11变量GA混合优化之程序—fmincon—搜索算法

2.含翅膀形貌学和运动学参数(人为设计谐波运动学规律)共计11个变量

3.功率调用函数和气动力调用函数一起调用同一个函数Aero_F_M_fruitfly——程序较简洁

4.变量约束区间改小——注意数据的上下限修改——直指频率约束f∈[150,260];

5.kenimatics_wing_and_AoA_fruitfly_sim输出(1000*9)矩阵

6.采用了hybrid_GA_fminsearch_wings_morphology_6原程序段来修改。



![laerodynamic_force](https://github.com/xijunke/aerodynamic_moment_model2_2_FCoeff_optimal/blob/master/pic_png_tif_eps_pdf/%E8%AE%A1%E7%AE%97%E5%92%8C%E5%AE%9E%E6%B5%8B%E5%9E%82%E7%9B%B4%E5%8A%9B%E5%92%8C%E6%B0%B4%E5%B9%B3%E5%8A%9B%E7%9A%84%E5%AF%B9%E6%AF%941.png)

![laerodynamic_force](https://github.com/xijunke/aerodynamic_moment_model2_2_FCoeff_optimal/blob/master/pic_png_tif_eps_pdf/%E8%AE%A1%E7%AE%97%E5%92%8C%E5%AE%9E%E6%B5%8B%E5%9E%82%E7%9B%B4%E5%8A%9B%E5%92%8C%E6%B0%B4%E5%B9%B3%E5%8A%9B%E7%9A%84%E5%AF%B9%E6%AF%942.png)

![laerodynamic_force](https://github.com/xijunke/aerodynamic_moment_model2_2_FCoeff_optimal/blob/master/pic_png_tif_eps_pdf/%E8%AE%A1%E7%AE%97%E5%92%8C%E5%AE%9E%E6%B5%8B%E5%9E%82%E7%9B%B4%E5%8A%9B%E5%92%8C%E6%B0%B4%E5%B9%B3%E5%8A%9B%E7%9A%84%E5%AF%B9%E6%AF%943.png)

![laerodynamic_force](https://github.com/xijunke/aerodynamic_moment_model2_2_FCoeff_optimal/blob/master/pic_png_tif_eps_pdf/%E8%AE%A1%E7%AE%97%E5%92%8C%E5%AE%9E%E6%B5%8B%E5%9E%82%E7%9B%B4%E5%8A%9B%E5%92%8C%E6%B0%B4%E5%B9%B3%E5%8A%9B%E7%9A%84%E5%AF%B9%E6%AF%944.png)

![laerodynamic_force](https://github.com/xijunke/aerodynamic_moment_model2_2_FCoeff_optimal/blob/master/pic_png_tif_eps_pdf/%E6%B3%95%E5%90%91%E5%90%88%E5%8A%9B%E5%88%86%E8%A7%A3%E5%88%B0%E5%9E%82%E7%9B%B4%E6%96%B9%E5%90%91%E5%92%8C%E6%B0%B4%E5%B9%B3%E6%96%B9%E5%90%91%E7%9A%84%E5%88%86%E9%87%8F%E5%8A%9B%E9%9A%8F%E6%97%B6%E9%97%B4%E7%9A%84%E5%8F%98%E5%8C%96%E8%A7%84%E5%BE%8B%E4%B8%8E%E5%AE%9E%E9%AA%8C%E6%B5%8B%E8%AF%95%E7%BB%93%E6%9E%9C%E7%9A%84%E5%AF%B9%E6%AF%94-2.png)

<div align=center>
<img src="https://github.com/xijunke/aerodynamic_moment_model2_2_FCoeff_optimal/blob/master/pic_png_tif_eps_pdf/%E6%B3%95%E5%90%91%E5%90%88%E5%8A%9B%E5%88%86%E8%A7%A3%E5%88%B0%E5%9E%82%E7%9B%B4%E6%96%B9%E5%90%91%E5%92%8C%E6%B0%B4%E5%B9%B3%E6%96%B9%E5%90%91%E7%9A%84%E5%88%86%E9%87%8F%E5%8A%9B%E9%9A%8F%E6%97%B6%E9%97%B4%E7%9A%84%E5%8F%98%E5%8C%96%E8%A7%84%E5%BE%8B%E4%B8%8E%E5%AE%9E%E9%AA%8C%E6%B5%8B%E8%AF%95%E7%BB%93%E6%9E%9C%E7%9A%84%E5%AF%B9%E6%AF%94-3.png" width="1200" height="700"/>
</div>