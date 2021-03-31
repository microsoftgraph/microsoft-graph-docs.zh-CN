---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 访问评审中的每个决策项表示主体对资源的访问权限。 accessReviewInstanceDecisionItemResource 表示与决策项关联的资源。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 879a0b1f74fa08e0ae66e5aaf5ab45b9d96de397
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469743"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

访问评审中的每个决策项表示主体对资源的访问权限。 accessReviewInstanceDecisionItemResource 表示与决策项关联的资源。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|资源的显示名称|
|id|String|资源 ID|
|type|String|资源的类型。 类型包括：Group、ServicePrincipal、DirectoryRole、AzureRole、AccessPackageAssignmentPolicy。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
