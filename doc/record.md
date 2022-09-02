1. [ ] 时间戳:格式转换 单位转换
2. [ ] eigen:旋转4种转换 点映射
3. [ ] 时间分段:
4. [ ] 插值:线性和球形
5. [ ] tuple:获取元素

Affine3ftrans_1 = Eigen::Affine3f::Identity();

trans_1.rotate(base_angle_q_);

trans_1.translate(base_pos_);

Affine3ftrans_2 = Eigen::Affine3f::Identity();

trans_2.rotate(cur_angle_q_);

trans_2.translate(cur_pos_);

Vector3fcorrected_lidar_point =trans_1.inverse()*trans_2*lidar_point;




bug:

放在主目录,bag包不要有中文路径  source devel/setup.sh
