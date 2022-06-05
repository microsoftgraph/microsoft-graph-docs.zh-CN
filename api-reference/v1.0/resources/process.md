---
title: 进程资源类型
description: 包含与警报相关的进程的有状态信息。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1c290ed08adae9f9b995c5c24c398826a2bb1160
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900490"
---
# <a name="process-resource-type"></a>进程资源类型

命名空间：microsoft.graph

包含与警报相关的进程的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|accountName|字符串|用户帐户标识符 (进程在) 下运行的用户帐户上下文，例如 AccountName、SID 等。|
|commandLine|String|包含所有参数的完整进程调用命令行。|
|createdDateTime|DateTimeOffset|开始此过程的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|fileHash|[fileHash](filehash.md)|包含文件哈希 (加密和位置敏感) 的复杂类型。|
|integrityLevel|processIntegrityLevel|过程的完整性级别。 可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|Boolean|如此 如果进程被提升。|
|name|字符串|进程的映像文件的名称。|
|parentProcessCreatedDateTime|DateTimeOffset|启动父进程的 DateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|parentProcessId|Int32|父进程的进程 ID (PID) 。|
|parentProcessName|字符串|父进程的映像文件的名称。|
|路径|String|完整路径，包括文件名。|
|processId|Int32|进程 ID (进程的 PID) 。|

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

