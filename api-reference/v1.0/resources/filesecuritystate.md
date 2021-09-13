---
title: fileSecurityState 资源类型
description: 包含有关未处理 (警报) 文件的信息。
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2db9d028c6a1550886a956bbfaad3bb3141f3141
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078859"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState 资源类型

命名空间：microsoft.graph

包含有关未处理 (警报) 文件的信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|包含文件哈希的复杂类型 (加密和位置敏感) 。|
|name|String|文件名 (路径) 。|
|路径|String|file/imageFile 的完整文件路径。|
|riskScore|String|警报文件的提供程序生成/计算的风险评分。 建议的值范围为 0-1，等于百分比。|

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

