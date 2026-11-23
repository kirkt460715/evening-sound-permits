# 夜间活动声学资料

该项目保存节目许可、声学观测及住户影响范围的合成资料。`data/acoustics.json` 保留许可版次、设备下限、停演和无节目对照时窗，供夜场排期人员讨论使用。

`data/permit-history.json` 提供有演出及安静对照的观测窗。没有活动实演记录的日期，在该窗口没有节目。声级字段为覆盖时段内的等效声级，`below_limit` 表示只知道读数低于设备量程。住户规则同时给出单窗和整晚的上限。

要求 Python 3.11 或更新版本。运行基线检查可使用 `python3 -m unittest discover -s tests`。`src/records.py` 提供基础 JSON 资料读取能力。
