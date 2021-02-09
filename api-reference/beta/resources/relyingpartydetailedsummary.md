---
title: relyingPartyDetailedSummary 资源类型
description: 表示 AD FS 中的信赖方。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a19132396f88797735801ee782c3c13e12a5e2ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161122"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>relyingPartyDetailedSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用 Active Directory 联合身份验证服务 (AD FS) 配置的信赖方、其聚合使用情况，以及信赖方配置是否可以迁移到 Azure Active Directory。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | 检索 **relyyPartyDetailedSummary 对象** 的列表。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。 在 API 级别生成的唯一标识符。| 
|relyingPartyId|String|此标识符用于标识此联合身份验证服务的信赖方。 它用于向信赖方发出声明。|
|服务 Id|String|唯一标识 Active Directory 林。|
|migrationStatus|string| 指示应用程序是否可以移动到 Azure AD 或需要进行更多调查。 可取值为：`ready`、`needsReview`、`additionalStepsRequired`。|
|migrationValidationDetails|[keyValuePair](keyvaluepair.md) 集合|指定对应用程序配置详细信息执行的所有验证检查，以评估应用程序是否已准备好移动到 Azure AD。 可能的名称是： `AdditionalWSFedEndpointCheckResult` ， ， ， ， ， ， ， ，  `AllowedAuthenticationClassReferencesCheckResult` ， `AlwaysRequireAuthenticationCheckResult`   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` 。 可能的结果值为 `0` ， `1` 或 `2` 。 `0` 验证检查通过时、 `1` 验证检查失败时以及验证 `2` 检查为警告时。 |
|relyingPartyName|String|Internet 上使用标识提供程序对想要登录的用户进行身份验证的应用程序或其他实体的名称。|
|failedSignInCount|Int64| 指定时段内 Active Directory 联合身份验证服务登录失败的数量。 |
|replyUrls|String 集合|指定信赖方希望在何处接收令牌。|
|signInSuccessRate|双精度|在指定的 (Active Directory 联合身份验证服务上成功登录) 成功登录数 + 失败登录数。|
|successfulSignInCount|Int64|Active Directory 联合身份验证服务上成功登录的数量。|
|totalSignInCount|Int64|指定时段内 Active Directory 联合身份验证服务上登录成功 + 失败登录失败的数量。|
|uniqueUserCount|Int64|已登录到应用程序的唯一用户数。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "keyProperty": "id"
}-->

```json
{
  "failedSignInCount": 10,
  "id": "String (identifier)",
  "migrationStatus": "ready | needsReview | additionalStepsRequired",
  "migrationValidationDetails": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": ["String"],
  "serviceId": "String (identifier)",
  "signInSuccessRate": 90.0,
  "successfulSignInCount": 90,
  "totalSignInCount": 100,
  "uniqueUserCount": 10
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relyingPartyDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


