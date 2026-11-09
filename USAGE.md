# 使用说明

## 适用任务

市场团队可导出全部家长手机号，兼职顾问账号在离职后仍可使用。

## 准备输入

系统与表格清单、字段字典、用户角色、业务流程、共享方式、供应商、保留策略、现有权限。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 定义范围
2. 盘点字段与系统
3. 映射流程和角色
4. 识别敏感/未成年人数据
5. 权限差距
6. 整改与复核

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

数据负责人/IT/法务复核学生数据字段、访问权限、供应商、日志和删除后，成果才可进入正式业务使用。
