---
title: resultTemplateOption 资源类型
description: 提供呈现连接器搜索结果的搜索显示布局选项。
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 404051f4eeee68ca3d5f5eb3ac6b84a23a331515
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211231"
---
# <a name="resulttemplateoption-resource-type"></a>resultTemplateOption 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用于呈现连接器搜索结果的搜索结果模板选项。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|enableResultTemplate|Boolean|指示是否启用搜索显示布局。 如果启用，用户将获取结果模板，以在响应 的 **resultTemplates** 属性中呈现 [搜索结果内容](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)。 结果模板基于自适应 [卡片](https://adaptivecards.io/)。 此属性可选。|


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
    "enableResultTemplate": true
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
