---
title: displayTemplate 资源类型
description: 定义内容的外观以及决定何时显示模板的条件。
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a20b9935ad142fce0a1b1fcd2a47e608a0fec670
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788764"
---
# <a name="displaytemplate-resource-type"></a>displayTemplate 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义内容的外观以及决定何时显示模板的条件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|显示模板的文本标识符;例如， `contosoTickets`. 最大 16 个字符。 仅允许字母数字字符。 |
|布局|[microsoft.graph.Json](../resources/intune-mam-json.md)|内容外观的定义，由 [自适应卡片](/adaptive-cards/authoring-cards/getting-started)表示，该卡片是 JSON 序列化卡片对象模型。|
|priority|Int32|定义显示模板的优先级。 优先级为 1 的显示模板在优先级为 4 的模板之前进行评估。 支持优先级值的差距。 必须是正值。|
|规则|[microsoft.graph.externalConnectors.propertyRule](../resources/externalconnectors-propertyrule.md) 集合|指定基于项架构选择此显示模板的其他规则。 可选。|

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