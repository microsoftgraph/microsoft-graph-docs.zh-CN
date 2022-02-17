---
title: resultTemplate 资源类型
description: 表示 resultTemplateIds 和关联值的字典，其中包括结果模板的名称和 JSON 架构。
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f6c3583ce13da2bc1c94325ed4a7db7353f329f0
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879269"
---
# <a name="resulttemplate-resource-type"></a>resultTemplate 资源类型

命名空间：microsoft.graph

表示 **resultTemplateIds** 和关联值的字典，其中包括结果模板的名称和 JSON 架构。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|body|Json|结果模板的 JSON 架构。|
|displayName|String|结果模板的名称。|
|注册表项|String|结果模板的 ID。 **key** 属性必须映射到 [searchHit](searchhit.md) 集合中的 **resultTemplateId**。|

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
                        "body": {"@odata.type": "microsoft.graph.Json"}
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


