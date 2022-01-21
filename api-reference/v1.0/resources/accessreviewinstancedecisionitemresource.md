---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 表示与决策项关联的资源。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fadfa73ca826c7f38ea179e80abf429c9092e071
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161107"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource 资源类型

命名空间：microsoft.graph

访问评审中的每个决策项表示主体对资源的访问权限。 资源由 accessReviewInstanceDecisionItemResource 对象标识。 

[accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionitemresource.md)是允许传入其他属性的开放类型，并且是以下资源的基础类型[：accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource、accessReviewInstanceDecisionItemAzureRoleResource](accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource.md)和[accessReviewInstanceDecisionItemServicePrincipalResource](accessreviewinstancedecisionitemserviceprincipalresource.md)。 [](accessreviewinstancedecisionitemazureroleresource.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|资源的显示名称|
|id|String|资源的标识符|
|type|String|资源的类型。 类型包括 `Group` `ServicePrincipal` `DirectoryRole` ：、、、、。 `AzureRole` `AccessPackageAssignmentPolicy`|

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
