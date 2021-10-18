---
title: subjectRightsRequestStageDetail 资源类型
description: 表示主题权限请求的阶段的属性
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2d4f62a704b115e9fb8a85525bb4cae818eb7a2
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60444708"
---
# <a name="subjectrightsrequeststagedetail-resource-type"></a>subjectRightsRequestStageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示主题权限请求的阶段的属性。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|[publicError](../resources/publicerror.md)|描述当前阶段的错误（如果有）。|
|stage|subjectRightsRequestStage|主体权限请求的阶段。 可取值为：`contentRetrieval`、`contentReview`、`generateReport`、`contentDeletion`、`caseResolved`、`unknownFutureValue`。|
|status|subjectRightsRequestStageStatus|当前阶段的状态。 可取值为：`notStarted`、`current`、`completed`、`failed`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestStageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestStageDetail",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "stage": "microsoft.graph.subjectRightsRequestStage",
  "status": "microsoft.graph.subjectRightsRequestStageStatus"
}
```

