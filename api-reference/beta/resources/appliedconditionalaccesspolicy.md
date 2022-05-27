---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与相应登录活动触发的已应用条件访问策略或策略相关的属性。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fe1f31555c2ea809d50faf87a1041f527a5ddc74
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695333"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>appliedConditionalAccessPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示与相应登录活动触发的已应用条件访问策略或策略相关的属性。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|authenticationStrength|[authenticationStrength](authenticationstrength.md)| 条件访问策略中强制实施的自定义身份验证强度。|
|conditionsNotSatisfied|conditionalAccessConditions|指不满足的条件访问策略条件。 可能的值为：`none`、、`application`、`devicePlatform``users`、`location`、`clientType`、`signInRisk`、`userRisk`、`time``deviceState`、`client``ipAddressSeenByAzureAD`、、`ipAddressSeenByResourceProvider`、、`servicePrincipals``servicePrincipalRisk``unknownFutureValue` 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的以下值： `servicePrincipals``servicePrincipalRisk`|
|conditionsSatisfied|conditionalAccessConditions|指满足的条件访问策略条件。 可能的值为：`none`、、`application`、`devicePlatform``users`、`location`、`clientType`、`signInRisk`、`userRisk`、`time``deviceState`、`client``ipAddressSeenByAzureAD`、、`ipAddressSeenByResourceProvider`、、`servicePrincipals``servicePrincipalRisk``unknownFutureValue` 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的以下值： `servicePrincipals``servicePrincipalRisk`|
|displayName|String|条件访问策略的名称。|
|enforcedGrantControls|String collection|引用条件访问策略强制实施的授权控件 (示例：“需要多重身份验证”) 。|
|enforcedSessionControls|String collection|引用条件访问策略 (示例强制实施的会话控件：“需要应用强制控制”) 。|
|excludeRulesSatisfied|[conditionalAccessRuleSatisfied](conditionalaccessrulesatisfied.md) 集合|包含条件访问策略中每个匹配的排除条件的键值对的列表。 示例： `[{"devicePlatform" : "DevicePlatform"}]` 表示策略未应用，因为 DevicePlatform 条件是匹配的。|
|id|String|条件访问策略的标识符。|
|includeRulesSatisfied|[conditionalAccessRuleSatisfied](conditionalaccessrulesatisfied.md) 集合|条件访问策略中包含每个匹配的包含条件的键值对的列表。 示例： `[{ "application" : "AllApps"}, {"users": "Group"}]`这意味着应用程序条件是一个匹配项，因为包括 AllApps *，* 而用户条件是匹配的，因为用户是包含的组规则的一部分。|
|result|appliedConditionalAccessPolicyResult| 指示已触发的 CA 策略的结果。 可能的值是：`success`， `notApplied` `failure` (策略未应用，因为) 不符合策略条件，`notEnabled` (这是由于禁用状态下的策略) 、`unknown`、`unknownFutureValue`、`reportOnlySuccess`、、 `reportOnlyNotApplied``reportOnlyInterrupted``reportOnlyFailure` 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的以下值： `reportOnlySuccess`， ， `reportOnlyFailure`， `reportOnlyNotApplied`。 `reportOnlyInterrupted`|
|sessionControlsNotSatisfied|String collection|指登录活动不满足的会话控件。  (示例： `Application enforced Restrictions`) 。|




## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "@odata.type": "#microsoft.graph.appliedConditionalAccessPolicy",
  "id": "String (identifier)",
  "authenticationStrength": {"@odata.type": "microsoft.graph.authenticationStrength"},
  "displayName": "String",
  "enforcedGrantControls": [
    "String"
  ],
  "enforcedSessionControls": [
    "String"
  ],
  "conditionsSatisfied": "String",
  "conditionsNotSatisfied": "String",
  "includeRulesSatisfied": [
    {
      "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
    }
  ],
  "excludeRulesSatisfied": [
    {
      "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
    }
  ],
  "result": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
