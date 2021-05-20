---
title: conditionalAccess 资源类型
description: '**conditionalaccess** 资源是 Conditinal Access 对象模型的入口点。 它不包含任何可用属性。'
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3683965cda79f003cb5e548101272d869be902b8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547411"
---
# <a name="conditionalaccess-resource-type"></a>conditionalaccess 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**conditionalAccess** 资源是条件访问对象模型的入口点。 它不包含任何可用属性。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) |[conditionalAccessPolicy](conditionalaccesspolicy.md)| 通过发布到 **conditionalAccessPolicy** 集合创建新的 conditionalAccessPolicy。|
|[创建 namedLocations](../api/conditionalaccessroot-post-namedlocations.md) |[namedLocation](namedlocation.md)| 通过发布到 **namedLocations** 集合创建新的 namedLocations。|
|[创建 authenticationContextClassReferences](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md)|[authenticationContextClassReferences](authenticationcontextclassreference.md)|通过发布到 **authenticationContextClassReferences** 集合创建新的 authenticationContextClassReferences。|


## <a name="properties"></a>属性

conditionalAccess 资源是条件访问对象模型的入口点，不包含任何属性。

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|conditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合| 只读。 可为 NULL。 返回指定的条件访问策略的集合。|
|namedLocations|[namedLocations](namedlocation.md) 集合| 只读。 可为 NULL。 返回指定命名位置的集合。|
|authenticationContextClassReferences|[authenticationContextClassReferences](authenticationcontextclassreference.md) 集合|只读。 可为 NULL。 返回指定的身份验证上下文类引用的集合。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditional access resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

