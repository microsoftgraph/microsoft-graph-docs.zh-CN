---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改以及更改注册表项的过程的信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 095d962ffcf09535042eda9f6ccf532351c091e9
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176722"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState 资源类型

命名空间：microsoft.graph

包含有关与警报相关的注册表项更改以及更改注册表项的过程的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|蜂巢|registryHive|[Windows注册表配置文件](/windows/desktop/sysinfo/registry-hives)： <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>\\HKEY_USERS。默认。</li></ul> 可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。|
|注册表项|String|当前 (，即更改) 注册表项 (排除 HIVE) 。|
|oldKey|String|以前的 (，即在更改注册表项之前，) 注册表项 (排除 HIVE) 。|
|oldValueData|String|以前的 (，即更改) 注册表项值数据之前 (内容) 。|
|oldValueName|String|以前的 (，即在更改注册表项值名称) 之前。|
|操作|registryOperation|更改注册表项名称和/或值的操作。 可能的值是：`unknown`、`create`、`modify`、`delete`。|
|processId|Int32|修改注册表项的进程的进程 ID (PID)  (进程详细信息将显示在警报“进程”集合) 中。|
|valueData|字符串|当前 (，即更改) 注册表项值数据 (内容) 。|
|valueName|字符串|当前 (，即已更改) 注册表项值名称|
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


