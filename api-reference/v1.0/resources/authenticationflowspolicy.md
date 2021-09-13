---
title: authenticationFlowsPolicy 资源类型
description: '表示租户级别的自助注册体验策略配置，允许外部用户请求注册以进行批准。 '
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 108b326010749235a2ecd631a4287d895de4ff71
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127057"
---
# <a name="authenticationflowspolicy-resource-type"></a>authenticationFlowsPolicy 资源类型

命名空间：microsoft.graph

表示租户级别的[自助注册体验策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行批准。 它包含有关 ID、显示名称和说明的信息，并指示是否对该策略启用了自助注册。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取身份验证流策略](../api/authenticationflowspolicy-get.md)|authenticationFlowsPolicy|获取身份验证流策略配置。|
|[更新身份验证流策略](../api/authenticationflowspolicy-update.md)|authenticationFlowsPolicy|更新身份验证流策略配置。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:-------|:---|:----------|
|id|字符串| 继承的属性。 身份验证流策略的标识符。 可选。 只读。
|displayName|字符串| 继承的属性。 策略的用户可读名称。 可选。 只读。|
|说明|字符串|继承的属性。 策略说明。 可选。 只读。|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |包含用于传达是否已启用或禁用自助注册的 [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) 设置。 可选。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```
