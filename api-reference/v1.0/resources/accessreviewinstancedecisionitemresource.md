---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 表示与决策项关联的资源。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3c51c0a4edf32bd090f78a6a921d0a246c0d33ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025627"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource 资源类型

命名空间：microsoft.graph

访问评审中的每个决策项表示主体对资源的访问权限。 accessReviewInstanceDecisionItemResource 对象表示与决策项关联的资源。

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
