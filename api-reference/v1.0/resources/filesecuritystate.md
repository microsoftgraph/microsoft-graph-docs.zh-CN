---
title: fileSecurityState 资源类型
description: 包含有关未处理 (警报) 文件的信息。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ac694c40e2f8a0a126d7849cf0131f4955af27d9e96aab73c30ead2d20ad42e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218721"
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

