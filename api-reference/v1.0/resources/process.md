---
title: 进程资源类型
description: 包含有关与警报相关的进程的有状态信息。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5fa15502d380d651128f55e6854bfe3592a290d1fb413b591a3f8f2571dca19f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222712"
---
# <a name="process-resource-type"></a>进程资源类型

命名空间：microsoft.graph

包含有关与警报相关的进程的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|accountName|String|用户帐户标识符 (进程在) 下运行，例如 AccountName、SID 等。|
|commandLine|String|包含所有参数的完整进程调用命令行。|
|createdDateTime|DateTimeOffset|启动进程的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|fileHash|[fileHash](filehash.md)|包含文件哈希的复杂类型 (加密和位置敏感) 。|
|integrityLevel|processIntegrityLevel|过程的完整性级别。 可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|Boolean|如果进程已提升，则其为 True。|
|name|String|进程的图像文件的名称。|
|parentProcessCreatedDateTime|DateTimeOffset|父进程的启动日期/时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|parentProcessId|Int32|进程 ID (PID) 的 PID。|
|parentProcessName|String|父进程的图像文件的名称。|
|路径|String|完整路径，包括文件名。|
|processId|Int32|进程 ID (PID) 进程。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

