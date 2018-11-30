---
title: registryKeyState 资源类型
description: 包含有关注册表的关键更改与通知，并更改的注册表项的过程信息。
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009510"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState 资源类型

包含有关注册表的关键更改与通知，并更改的注册表项的过程信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|配置单元|registryHive|[Windows 注册表配置单元](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)中： <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>读</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\。默认值。</li></ul> 可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault`。|
|Key|字符串|当前的 （即更改） 的注册表项 （排除配置单元）。|
|oldKey|字符串|（即更改之前） 以前注册表项 （排除配置单元）。|
|oldValueData|字符串|（即更改之前） 以前注册表项的值数据 （内容）。|
|oldValueName|字符串|（即更改之前） 以前注册表项的值名称。|
|操作|registryOperation|更改的注册表项名称和/或值的操作。 可取值为：`unknown`、`create`、`modify`、`delete`。|
|processId|Int32|处理 ID (PID) 的过程的修改注册表项 （详细信息将显示通知进程集合中的过程）。|
|valueData|字符串|当前 （即更改） 的注册表项的值数据 （内容）。|
|数值名称|字符串|当前 （即更改） 的注册表项的值名称|
|valueType|registryValueType|[注册表项的值类型](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> 可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。|

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