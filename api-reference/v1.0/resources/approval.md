---
title: 审批资源类型
description: 与 userConsentRequest 或 accessPackageAssignmentRequest 关联的审批对象。
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 812c2315593abdc0556fcf2a5f2d545299999fc1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395858"
---
# <a name="approval-resource-type"></a>审批资源类型

命名空间：microsoft.graph

表示与请求关联的决策的审批对象。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取审批](../api/approval-get.md) | [审批](approval.md) | 在权利管理 **中检索审批** 对象的属性。 |
|[filterByCurrentUser](../api/approval-filterbycurrentuser.md)| [审批](approval.md) 集合| 在 **权利管理** 中检索审批者的批准对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|审批决策的标识符。|

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
