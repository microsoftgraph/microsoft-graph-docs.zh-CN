---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 表示与决策项关联的资源。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b9b411d1b101d1f2fdc746d2bfb70d0dae8ede9b
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226552"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource 资源类型

命名空间：microsoft.graph

访问评审中的每个决策项表示主体对由 accessReviewInstanceDecisionItemResource 对象标识的资源的访问权限。 accessReviewInstanceDecisionItemResource 是允许传入其他属性的开放类型。

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
