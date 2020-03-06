---
title: fileSecurityState 资源类型
description: 包含有关与警报相关的文件（不处理）的信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc9d05e875104469a25ee742635ea8e86682d9e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531426"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState 资源类型

命名空间：microsoft.graph

包含有关与警报相关的文件（不处理）的信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|包含文件哈希（加密和位置敏感）的复杂类型。|
|name|字符串|文件名（不含路径）。|
|路径|String|文件/imageFile 的完整文件路径。|
|riskScore|字符串|通知文件的提供程序生成/计算风险分数。 建议的值范围为0-1，这相当于一个百分比。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
