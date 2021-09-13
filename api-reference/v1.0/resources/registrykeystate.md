---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改以及更改注册表项的过程的信息。
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dff818881dbbaa2fe079a34850894251cb689bf3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044270"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState 资源类型

命名空间：microsoft.graph

包含有关与警报相关的注册表项更改以及更改注册表项的过程的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hive|registryHive|注册表[Windows配置单元：](/windows/desktop/sysinfo/registry-hives) <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS \\ 。默认值。</li></ul> 可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。|
|注册表项|String|当前 (，即更改) 注册表项 (HIVE) 。|
|oldKey|String|以前的 (，即更改之前) 注册表项 (HIVE) 。|
|oldValueData|String|上 (，即更改之前) 注册表项值数据 (内容) 。|
|oldValueName|String|上 (项，即更改) 注册表项值名称之前。|
|operation|registryOperation|更改注册表项名称和/或值的操作。 可取值为：`unknown`、`create`、`modify`、`delete`。|
|processId|Int32|进程 ID (PID) 修改了注册表项的进程的详细信息 (将显示在警报"进程"集合) 。|
|valueData|String|当前 (，即更改) 注册表项值数据 (内容) 。|
|valueName|String|当前 (，即更改) 注册表项值名称|
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

