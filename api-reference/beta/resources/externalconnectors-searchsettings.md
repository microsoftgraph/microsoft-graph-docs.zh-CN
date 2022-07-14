---
title: searchSettings 资源类型
description: 通过连接器内容收集与搜索相关的所有可配置设置。
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f0915d57f0c49199f0273b8c44d5f60b2d78531c
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788631"
---
# <a name="searchsettings-resource-type"></a>searchSettings 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过连接器内容收集与搜索相关的所有可配置设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|searchResultTemplates|[microsoft.graph.externalConnectors.displayTemplate](../resources/externalconnectors-displaytemplate.md) 集合|使开发人员能够定义内容的外观并配置条件，这些条件决定了何时应显示模板。 每个连接最多 2 个搜索结果模板。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.searchSettings"
}
-->
``` json
{
  "searchResultTemplates": [
    {
      "id": "String (identifier)",
      "rules": [
        {
          "property": "itemTitle",
          "operation": "contains",
          "valuesJoinedBy": "or",
          "values": [
              "contoso",
              "smart"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "A contoso ticket."}]},
      "priority": 0
    },
        {
      "id": "String (identifier)",
      "rules": [
        {
          "property": "itemDescription",
          "operation": "contains",
          "valuesJoinedBy": "and",
          "values": [
              "contoso",
              "ticket"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "A contoso ticket."}]},
      "priority": 1
    }
  ]
}
```

