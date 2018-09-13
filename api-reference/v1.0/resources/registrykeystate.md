# <a name="registrykeystate-resource-type"></a>registryKeyState 资源类型

包含有关注册表项的更改与提示，以及如何更改注册表项的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hive|registryHive| [Windows 注册表配置单元](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)： <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\。默认值。</li></ul> 可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault`。|
|key|字符串|当前的 （更改后）的注册表项 （不含 HIVE）。|
|oldKey|字符串|更改之前的注册表项 （不含 HIVE）。|
|oldValueData|字符串|此前（即更改之前）的注册表项的值数据 （内容）。|
|oldValueName|字符串|此前（即更改之前）注册表项的值名称。|
|operation|registryOperation|更改的注册表项名称和/或值的操作。 可取值为：`unknown`、`create`、`modify`、`delete`。|
|processId|Int32|修改注册表项流程的流程 ID (PID)（ 流程详细信息将显示于通知的 'process' 集合中）。|
|valueData|字符串|当前 （即更改后）的注册表项的值数据 （内容）。|
|valueName|字符串|当前 （即更改后）的注册表项的值名称|
|valueType|registryValueType|[注册表项的值类型](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> 可能的值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->