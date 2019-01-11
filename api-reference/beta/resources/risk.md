---
title: 风险的资源类型
description: 汇聚风险级别、 风险状态和风险详细信息 risky 用户登录，或风险事件。
localization_priority: Normal
ms.openlocfilehash: da198ba27ca6cd0b762f322863f8c9bfd56a5cb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810666"
---
# <a name="risk-resource-type"></a>风险的资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

汇聚风险级别、 风险状态和风险详细信息 risky 用户登录，或风险事件。

## <a name="properties"></a>属性

| 属性   | 类型|Description|
|:---------------|:--------|:----------|
|`stateDetail`|riskDetail|提供原因后面的 risky 用户、 登录或风险事件特定状态。 可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。 值`none`是指的任何操作已执行上的用户或登录到目前为止。 |
|`riskLevelAggregated`|riskLevel|提供 risky 用户、 登录或风险事件的总体风险级别。 可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。 值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。|
|`riskLevelDuringSignIn`|riskLeve|登录过程中 （即基于实时风险事件） 提供登录的风险级别。 可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。 值`hidden`是指为 Azure AD 身份保护未启用登录。|
|`state`|riskState|提供 risky 用户、 登录或风险事件的风险状态。 可能的值为： `none`， `confirmedSafe`， `remediated`， `dismissed`， `atRisk`， `confirmedCompromised`， `unknownFutureValue`。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
