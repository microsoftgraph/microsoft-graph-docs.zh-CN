---
title: searchSettings 资源类型
description: 收集与搜索连接器内容相关的所有可配置设置。
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6750ce5ea8f6b74dd55e83dae1a8f22d04ebfc15
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214921"
---
# <a name="searchsettings-resource-type"></a>searchSettings 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

收集与搜索连接器内容相关的所有可配置设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|searchResultTemplates|[microsoft.graph.externalConnectors.displayTemplate](../resources/externalconnectors-displaytemplate.md) 集合|使开发人员能够定义内容的外观并配置规定应何时显示模板的条件。|

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

