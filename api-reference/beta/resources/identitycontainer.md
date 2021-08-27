---
title: identityContainer 资源类型
description: 表示Azure Active Directory （Azure AD） 和 Azure AD B2C 租户的外部标识中不同功能的入口点。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 44c11b4e2280a38f243898a0e5b19dd5a63a1440
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2021
ms.locfileid: "58668080"
---
# <a name="identitycontainer-resource-type"></a>identityContainer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Azure Active Directory（Azure AD）和Azure AD B2C租户的 [外部标识](/azure/active-directory/external-identities/) 中不同功能的入口点。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|apiConnectors|[identityApiConnector](identityApiConnector.md) 集合|表示 API 连接器的入口点。|
|b2cUserFlows|[b2cIdentityUserFlow](b2cIdentityUserFlow.md) 集合|表示 B2C 标识用户流的入口点。|
|b2xUserFlows|[b2xIdentityUserFlow](b2xIdentityUserFlow.md) 集合| 表示 B2X 和自助注册标识用户流的入口点。|
|identityProviders|[identityProviderBase](identityProviderBase.md) 集合| 表示标识提供程序基的入口点。|
|userFlowAttributes|[identityUserFlowAttribute](identityUserFlowAttribute.md) 集合| 表示标识用户流属性的入口点。|
|continuousAccessEvaluationPolicy|[continuousAccessEvaluationPolicy](continuousAccessEvaluationPolicy.md)| 表示连续访问评估策略的入口点。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityContainer"
}
```
