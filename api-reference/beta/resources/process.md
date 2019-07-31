---
title: 进程资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6b67ec28dadb09442c5e3d66b6c03c54db821a85
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965689"
---
# <a name="process-resource-type"></a>进程资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关与警报相关的进程的状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|帐户|String|用户帐户标识符 (进程在其下运行的用户帐户上下文) 例如, AccountName、SID 等。|
|commandLine|String|完整的过程调用命令行, 包括所有参数。|
|createdDateTime|DateTimeOffset|启动进程的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|fileHash|[fileHash](filehash.md)|包含文件哈希 (加密和位置敏感) 的复杂类型。|
|integrityLevel|processIntegrityLevel|进程的完整性级别。 可取值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|Boolean|如果进程已提升, 则为 True。|
|name|String|进程的图像文件的名称。|
|parentProcessCreatedDateTime|DateTimeOffset|父进程已启动的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|parentProcessId|Int32|父进程的进程 ID (PID)。|
|parentProcessName|String|父进程的图像文件的名称。|
|路径|字符串|完整路径, 包括文件名。|
|processId|Int32|进程的进程 ID (PID)。|

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
