---
title: resultTemplate 资源类型
description: resultTemplateIds 和关联值的字典，其中包括结果模板的名称和 JSON 架构。
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
---

# <a name="resulttemplate-resource-type"></a>resultTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**resultTemplateIds** 和相关值的字典，其中包括结果模板的名称和 JSON 架构。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|Key|String|结果模板的 ID。 它必须映射到 [searchHit](searchhit.md) 中的 **resultTemplateId**。|
|displayName|String|结果模板的名称。|
|body|Json|结果模板的 JSON 架构。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
   "resultTemplateId": {
      "displayName": "String",
      "body": "Json schema"
   }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


