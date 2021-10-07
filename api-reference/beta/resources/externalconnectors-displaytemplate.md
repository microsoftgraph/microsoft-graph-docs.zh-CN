---
title: displayTemplate 资源类型
description: 定义内容的外观以及规定何时应显示模板的条件。
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5138bb43bea3aec216dcb86ffc2f09eaec96e315
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214923"
---
# <a name="displaytemplate-resource-type"></a>displayTemplate 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义内容的外观以及规定何时应显示模板的条件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|显示模板的文本标识符;例如， `contosoTickets` 。|
|layout|[microsoft.graph.Json](../resources/intune-mam-json.md)|内容外观的定义，由自适应 [卡片](https://docs.microsoft.com/adaptive-cards/authoring-cards/getting-started)表示，该卡片是 JSON 序列化的卡片对象模型。|
|priority|Int32|定义显示模板的优先级。 优先级为 1 的显示模板先于优先级为 4 的模板进行评估。 支持优先级值中的间隔。|
|规则|[microsoft.graph.externalConnectors.propertyRule](../resources/externalconnectors-propertyrule.md) 集合|指定用于基于项目架构选择此显示模板的其他规则。 可选。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.displayTemplate"
}
-->
``` json
    {
      "id": "String",
      "rules": [
        {
          "property": "String",
          "operation": "String",
          "valuesJoinedBy": "String",
          "values": [
              "String",
              "String"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "String"}]},
      "priority": 0
    }
```

