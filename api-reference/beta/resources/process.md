---
title: 进程资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: db832c64fb62e6c5f72f49b1e147d8d7f282834f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722263"
---
# <a name="process-resource-type"></a>进程资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关与警报相关的过程的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|accountName|String|用户帐户标识符 (进程在) 下运行，例如 AccountName、SID 等。|
|commandLine|String|包含所有参数的完整进程调用命令行。|
|createdDateTime|DateTimeOffset|启动过程的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|fileHash|[fileHash](filehash.md)|包含文件哈希的复杂类型 (加密和位置敏感的) 。|
|integrityLevel|processIntegrityLevel|进程的完整性级别。 可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|布尔值|如果提升进程，则其为 True。|
|name|String|进程的图像文件的名称。|
|parentProcessCreatedDateTime|DateTimeOffset|启动父进程的 DateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|parentProcessId|Int32|进程 ID (PID) 父进程。|
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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


