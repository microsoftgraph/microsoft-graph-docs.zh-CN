---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改的信息, 以及更改了注册表项的过程。
localization_priority: Normal
ms.openlocfilehash: d07b0b6f502794154b400444eaf3854535e04547
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994424"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState 资源类型

包含有关与警报相关的注册表项更改的信息, 以及更改了注册表项的过程。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|配置单元|registryHive|[Windows 注册表配置单元](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives): <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\。设置.</li></ul> 可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。|
|注册表项|String|当前 (如已更改) 的注册表项 (不包括配置单元)。|
|oldKey|String|上一个 (即 "更改前") 注册表项 (不包括 HIVE)。|
|oldValueData|String|以前的 (即更改之前) 注册表项值数据 (内容)。|
|oldValueName|String|以前的注册表项值名称 (即 "更改前")。|
|操作|registryOperation|更改注册表项名称和/或值的操作。 可取值为：`unknown`、`create`、`modify`、`delete`。|
|processId|Int32|修改注册表项的进程的进程 ID (PID) (进程详细信息将显示在警报的 "进程" 集合中)。|
|valueData|String|当前 (如已更改) 的注册表项值数据 (内容)。|
|等值|String|当前 (如已更改) 的注册表项值名称|
|valueType|registryValueType|[注册表项值类型](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> 可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。|

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
