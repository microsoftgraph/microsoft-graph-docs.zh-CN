---
title: resultTemplateOption 资源类型
description: 提供用于呈现来自连接器的搜索结果的搜索结果模板选项。
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5f1e6b30a1730bfb0e4a667b51c93a47cc3dcb12
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878681"
---
# <a name="resulttemplateoption-resource-type"></a>resultTemplateOption 资源类型

命名空间：microsoft.graph

提供用于呈现来自连接器的搜索结果的搜索结果模板选项。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|enableResultTemplate|Boolean|指示是否启用搜索显示布局。 如果启用，用户将获取结果模板，以在响应的 **resultTemplates** 属性中呈现 [搜索结果内容](/graph/api/resources/searchresponse)。 结果模板基于自适应 [卡片](https://adaptivecards.io/)。 可选。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplateOption",
  "baseType": null
}-->

```json
 {
    "enableResultTemplate": "Boolean"
 }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplateOption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
