# rename_armature_to_ue_standard

## Blender script to rename armature bones to Unreal Engine standard naming convention.

### Supports:
- VRM (hips, spine, chest, shoulder, upper_arm/lower_arm, upper_leg/lower_leg, toes, fingers)
- Mixamo (mixamorig:Hips, mixamorig:Spine*, mixamorig:Left/Right*, Hand/Toe/Head Ends)
- Rigify Human (spine, shoulder, upper_arm/forearm, thigh/shin, toe, palm, fingers)

For Mixamo, finger/toe/head end bones are deleted.
For VRM/Rigify/Unknown, unmapped bones are standardized (e.g., .L/.R -> _l/_r, .00x -> _0x, lowercase).

---

## 操作步骤：选中骨骼进入编辑模式，将次脚本拖入Blender的脚本页面点击运行

- 需要选中骨骼在编辑模式下运行此脚本
- 支持骨骼类型: VRM / Rigify / Mixamo
- 注意：Mixamo骨骼会删除 头部/手指/脚趾 的_End末端骨骼
