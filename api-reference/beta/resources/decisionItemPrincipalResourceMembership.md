---
title: decisionItemPrincipalResourceMembership 资源类型
description: 访问评审中的每个决策都表示主体对资源的访问权限。 decisionItemPrincipalResourceMembership 对象公开主体对与 accessReviewInstanceDecisionItem 对象关联的资源的成员身份类型的详细信息。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9ff76ae47d8289827b9c6309288272d3b9c1e6c1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447574"
---
# <a name="decisionitemprincipalresourcemembership-resource-type"></a>decisionItemPrincipalResourceMembership 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

访问评审中的每个决策都表示主体对资源的访问权限。 **decisionItemPrincipalResourceMembership** 对象公开主体对与 [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 对象关联的资源的成员身份类型的详细信息。 例如，主体可以直接或间接访问资源。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|membershipType| decisionItemPrincipalResourceMembershipType | 主体对资源拥有的成员身份类型。 多值。 可能的值包括 `direct`、`indirect`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.decisionItemPrincipalResourceMembership",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.decisionItemPrincipalResourceMembership",
  "membershipType": "String",
}
```
