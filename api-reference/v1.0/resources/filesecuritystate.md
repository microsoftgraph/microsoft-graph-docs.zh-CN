---
title: fileSecurityState 资源类型
description: 包含有关与警报相关的文件 (不处理) 的信息。
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564790"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState 资源类型

包含有关与警报相关的文件 (不处理) 的信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|包含文件哈希 (加密和位置敏感) 的复杂类型。|
|name|String|文件名 (不含路径)。|
|路径|String|文件/imageFile 的完整文件路径。|
|riskScore|String|通知文件的提供程序生成/计算风险分数。 建议的值范围为 0-1, 这相当于一个百分比。|

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
