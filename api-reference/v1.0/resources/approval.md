---
title: 审批资源类型
description: 与 userConsentRequest 关联的审批对象。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b2917825104d30813f6ad98237dd68492e4a269481d1013458edb1038208430c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212219"
---
# <a name="approval-resource-type"></a>审批资源类型

命名空间：microsoft.graph

表示与请求关联的决策的审批对象。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|审批决策的标识符。|
|stages|[approvalStage](../resources/approvalstage.md) 集合|审批决策中的阶段集合。 |

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|stages|[approvalStage](../resources/approvalstage.md) 集合|审批决策中的阶段集合。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```
