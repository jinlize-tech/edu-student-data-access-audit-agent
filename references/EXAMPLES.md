# 学员数据地图与权限审计示例

## 典型场景

市场团队可导出全部家长手机号，兼职顾问账号在离职后仍可使用。

## 具体示例

Agent 标记越权访问和离职账号，优先建议关闭高敏导出，不自动读取或修改真实系统。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "systems_inventory": [
    {}
  ],
  "data_fields": [
    {}
  ],
  "user_roles": [
    {}
  ],
  "access_matrix": [
    {}
  ],
  "vendor_list": [
    {}
  ],
  "retention_policy": "保留与删除规则已核对（脱敏示例）",
  "student_data_categories": [
    {}
  ],
  "change_context": "变更背景已核对（脱敏示例）",
  "resume_mode": "new"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出学员数据地图、权限矩阵、整改优先级等核心成果。
5. 由数据负责人/IT/法务确认学生数据字段、访问权限、供应商、日志和删除后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
