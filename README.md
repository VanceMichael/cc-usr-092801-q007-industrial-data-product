# 工业数据产品授权与收益分配

管理工业数据产品版本、许可、调用计量、影响传播和收益分配。

## 参与方与事实

主要参与方包括数据资产运营团队、制造企业、数据贡献单位、合规审批人员、收益结算人员。领域资料记录以下已经确认的事实：

- 我国推进工业数据要素市场化配置
- 工业数据交易仍面临权属和收益分配问题
- 数据产品化需要安全流通和规则建设

## 业务约束

- 数据产品谱系
- 许可版本
- 调用计量
- 授权影响
- 收益守恒

`contracts/context.schema.json` 描述资料结构，`fixtures/context.json` 提供不含真实身份信息的示例，`src/industrial_data_context.py` 负责读取和校验这些资料。

## 开发命令

运行测试：

```bash
python3 -m unittest discover -s tests -v
```

编译检查：

```bash
python3 -m compileall -q src
```

两条命令只读取仓库内文件，不需要连接外部业务系统。
