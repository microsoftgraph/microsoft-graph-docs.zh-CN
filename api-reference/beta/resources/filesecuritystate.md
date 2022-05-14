---
title: fileSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: f080ecded6cf6716f985ccf06e885e9955c8525d
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420451"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关文件 (不处理与警报相关的) 的信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|包含文件哈希 (加密和位置敏感) 的复杂类型。|
|name|String|文件名 (没有路径) 。|
|路径|String|文件/imageFile 的完整文件路径。|
|riskScore|String|警报文件的提供程序生成/计算风险分数。 建议的值范围为 0-1，这等同于百分比。|

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


