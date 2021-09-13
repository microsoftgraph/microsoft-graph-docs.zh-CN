---
title: 审批资源类型
description: 与 userConsentRequest 关联的审批对象。
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f59736f7cdb4aed235eeb1fa5831e69024057d11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067610"
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
