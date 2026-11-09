# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `systems_inventory` | 系统与表格清单 | array | 是 |
| `data_fields` | 学生数据字段 | array | 是 |
| `user_roles` | 用户角色 | array | 是 |
| `access_matrix` | 现有访问矩阵 | array | 是 |
| `vendor_list` | 供应商与共享 | array | 否 |
| `retention_policy` | 保留与删除规则 | string | 是 |
| `student_data_categories` | 学生敏感数据类别 | array | 是 |
| `change_context` | 变更背景 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `学员数据地图`：结构化条目数组，不允许空壳或占位文本。
- `处理活动表`：结构化条目数组，不允许空壳或占位文本。
- `权限矩阵`：结构化条目数组，不允许空壳或占位文本。
- `共享清单`：结构化条目数组，不允许空壳或占位文本。
- `留存缺口`：结构化条目数组，不允许空壳或占位文本。
- `整改优先级`：结构化条目数组，不允许空壳或占位文本。
- `复测清单`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
