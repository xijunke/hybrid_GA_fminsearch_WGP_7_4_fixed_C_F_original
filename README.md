# Aerodynamic force，moment and power with/without including inertial force for Optimal Wing Geometry Parameters

## 由hybrid_GA_fminsearch_wings_morphology_6修改而来，20160106日之前该论文的一些气动力和力矩以及功率的计算程序有小错误

### 目前改程序已经修改，几近正确

0.hybrid_GA_fminsearch_WingM4_4_2由hybrid_GA_fminsearch_WingM4_4_1进化修改而来

1.该文件夹下为11变量GA混合优化之程序—fmincon—搜索算法

2.含翅膀形貌学和运动学参数(人为设计谐波运动学规律)共计11个变量

3.功率调用函数和气动力调用函数一起调用同一个函数Aero_F_M_fruitfly——程序较简洁

4.变量约束区间改小——注意数据的上下限修改——直指频率约束f∈[150,260];

5.kenimatics_wing_and_AoA_fruitfly_sim输出(1000*9)矩阵

6.采用了hybrid_GA_fminsearch_wings_morphology_6原程序段来修改。


## Aerodynamic force and power based on the original wing morphology parameters and motion data

## 针对原始翅膀形貌参数和运动数据的气动力和功率

![aerodynamic_forces_lift_and_thrust](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_force_power/png/aerodynamic_forces_lift_and_thrust.png)

![Aerodynamic power](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_force_power/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x_%7Brw%7D-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9F%E7%8E%87%E5%92%8C%E6%83%AF%E6%80%A7%E5%8A%9F%E7%8E%87_2.png)

![Aerodynamic power](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_force_power/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z_%7Brr%7D-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9F%E7%8E%87%E5%92%8C%E6%83%AF%E6%80%A7%E5%8A%9F%E7%8E%87_2.png)

## Aerodynamic forces and moments in wing plane frame

### 翅平面坐标下的气动力和力矩，含惯性力

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/with_inertial_force_moment/png/aerodynamic_normal_forces_3.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/with_inertial_force_moment/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A9_3.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/with_inertial_force_moment/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A9_6.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/with_inertial_force_moment/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A93.png)


### 翅平面坐标下的气动力和力矩，不含惯性力

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/without_inertial_force_moment/png/aerodynamic_normal_forces.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/without_inertial_force_moment/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A9.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/without_inertial_force_moment/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A9.png)


# Aero_F_M_for_flapping_ODE_solving_with_inertial_force_moment used for flapping dynamic ODE solving

# 用于计算拍打ODE方程的方案_含惯性力和力矩

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/aerodynamic_normal_forces_5.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/aerodynamic_normal_forces_5_%E8%99%9A%E8%B4%A8%E9%87%8F%E5%8A%9B%E5%8F%98%E5%90%91.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A9_5.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x_%7Brw%7D-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9F%E7%8E%87%E5%92%8C%E6%83%AF%E6%80%A7%E5%8A%9F%E7%8E%87_4.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A95.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z_%7Brr%7D-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9F%E7%8E%87%E5%92%8C%E6%83%AF%E6%80%A7%E5%8A%9F%E7%8E%87_4.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_flapping_ODE/png/%E9%92%88%E5%AF%B9%E6%9C%80%E4%BC%98%E7%BF%85%E8%86%80%E5%BD%A2%E8%B2%8C%E5%8F%82%E6%95%B0%E7%9A%84%E7%BF%85%E6%89%AD%E8%BD%AC%E5%8A%9F%E7%8E%87%E3%80%81%E6%8B%8D%E6%89%93%E5%8A%9F%E7%8E%87%E5%92%8C%E6%80%BB%E5%8A%9F%E7%8E%87%E8%BE%93%E5%87%BA3.png)


# Aero_F_M_for_pitch_ODE_solving_with_inertial_force_moment used for pitch dynamic ODE solving

# 用于计算扭转ODE方程的方案_含惯性力和力矩

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_pitch_ODE/png/aerodynamic_normal_forces_4.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_pitch_ODE/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A9_4.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_pitch_ODE/png/%E6%B2%BF%E7%9D%80%E6%89%AD%E8%BD%AC%E8%BD%B4x_%7Brw%7D-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9F%E7%8E%87%E5%92%8C%E6%83%AF%E6%80%A7%E5%8A%9F%E7%8E%87_3.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_pitch_ODE/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9B%E7%9F%A94.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_pitch_ODE/png/%E6%B2%BF%E7%9D%80%E6%8B%8D%E6%89%93%E8%BD%B4z_%7Brr%7D-axis%E7%9A%84%E6%B0%94%E5%8A%A8%E5%8A%9F%E7%8E%87%E5%92%8C%E6%83%AF%E6%80%A7%E5%8A%9F%E7%8E%87_3.png)

![aerodynamic_force](https://github.com/xijunke/hybrid_GA_fminsearch_WGP_7_4_fixed_C_F_original/blob/master/Pic_aerodynamic_forces_moments/Aero_F_M_with_inertial_force_moment_for_pitch_ODE/png/%E9%92%88%E5%AF%B9%E6%9C%80%E4%BC%98%E7%BF%85%E8%86%80%E5%BD%A2%E8%B2%8C%E5%8F%82%E6%95%B0%E7%9A%84%E7%BF%85%E6%89%AD%E8%BD%AC%E5%8A%9F%E7%8E%87%E3%80%81%E6%8B%8D%E6%89%93%E5%8A%9F%E7%8E%87%E5%92%8C%E6%80%BB%E5%8A%9F%E7%8E%87%E8%BE%93%E5%87%BA2.png)

