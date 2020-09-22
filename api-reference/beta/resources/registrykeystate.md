---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改的信息，以及更改了注册表项的过程。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: b5da3318a229ea46329466f3b403fec519ffbc61
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073430"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState 资源类型

命名空间：microsoft.graph

包含有关与警报相关的注册表项更改的信息，以及更改了注册表项的过程。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|配置单元|registryHive|[Windows 注册表配置单元](/windows/desktop/sysinfo/registry-hives)： <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE \SAM</li> <li>HKEY_LOCAL_MACHINE \Security</li> <li>HKEY_LOCAL_MACHINE \Software</li> <li>HKEY_LOCAL_MACHINE \System</li> <li>HKEY_USERS \\ 。设置.</li></ul> 可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。|
|注册表项|String|当前 (即) 注册表项更改 (排除配置单元) 。|
|oldKey|String|以前的 (，即在更改) 注册表项之前 (排除配置单元) 。|
|oldValueData|String|以前的 (，即在更改) 注册表项值数据 (内容) 之前。|
|oldValueName|String|以前的 (，即在更改) 注册表项值名称之前。|
|操作|registryOperation|更改注册表项名称和/或值的操作。 可取值为：`unknown`、`create`、`modify`、`delete`。|
|processId|Int32|进程 ID (PID) 修改注册表项 (进程详细信息将显示在警报的 "进程" 集合) 中。|
|valueData|String|当前 (即) 注册表项值数据 (内容) 更改。|
|等值|String|当前 (即) 注册表项值名称更改|
|valueType|registryValueType|[注册表项值类型](/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> 可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。|

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


