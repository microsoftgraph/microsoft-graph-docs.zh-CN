---
title: 审批资源类型
description: 与 userConsentRequest 关联的审批对象。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6d41146551586f681ebf5ed7fda735151f1efc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469541"
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
