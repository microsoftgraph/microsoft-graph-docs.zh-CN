---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 访问评审中的每个决策项都表示主体对资源的访问权限。 accessReviewInstanceDecisionItemResource 表示与决策项关联的资源。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f35317538a1cac512e6f3dfc0997bb721ac9681
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698147"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

访问评审中的每个决策项都表示主体对资源的访问权限。 资源由 accessReviewInstanceDecisionItemResource 对象标识。

[accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionitemresource.md) 是一种开放类型，允许传入其他属性，并且是以下资源的基础类型： [accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource](accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource.md)、 [accessReviewInstanceDecisionItemAzureRoleResource](accessreviewinstancedecisionitemazureroleresource.md) 和 [accessReviewInstanceDecisionItemServicePrincipalResource](accessreviewinstancedecisionitemserviceprincipalresource.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|资源的显示名称|
|id|String|资源 ID|
|type|字符串|资源的类型。 类型包括： `Group`， `ServicePrincipal`， `DirectoryRole`， `AzureRole`， 。 `AccessPackageAssignmentPolicy`|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
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
