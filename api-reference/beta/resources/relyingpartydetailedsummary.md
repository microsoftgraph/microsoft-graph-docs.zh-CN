---
title: relyingPartyDetailedSummary 资源类型
description: 表示 AD FS 中的信赖方。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6e840c47ed5170f95929d686fe9ff94be54ea1ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962110"
---
# <a name="relyingpartydetailedsummary-resource-type"></a>relyingPartyDetailedSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用 Active Directory 联合身份验证服务 (AD FS) 配置的信赖方、其聚合使用情况，以及信赖方配置是否可以迁移到 Azure Active Directory。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/relyingpartydetailedsummary-list.md) | [relyingPartyDetailedSummary](relyingpartydetailedsummary.md) | 检索 **relyingPartyDetailedSummary 对象** 的列表。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。 在 API 级别生成的唯一标识符。| 
|relyingPartyId|String|此标识符用于标识此联合身份验证服务的信赖方。 向信赖方发出声明时，会使用声明。|
|服务 Id|String|唯一标识 Active Directory 林。|
|migrationStatus|migrationStatus| 指示应用程序是否可以移动到 Azure AD 或需要更多调查。 可取值为：`ready`、`needsReview`、`additionalStepsRequired`、`unknownFutureValue`。|
|migrationValidationDetails|[keyValuePair](keyvaluepair.md) 集合|指定在应用程序配置详细信息上完成的所有验证检查，以评估应用程序是否已准备好移动到 Azure AD。|
|relyingPartyName|String|Internet 上使用标识提供程序对要登录的用户进行身份验证的应用程序或其他实体的名称。|
|failedSignInCount|Int64| 指定时段内 Active Directory 联合身份验证服务上的登录失败次数。 |
|replyUrls|String 集合|指定信赖方期望接收令牌的地方。|
|signInSuccessRate|双精度|在指定的 (Active Directory 联合身份验证服务上成功登录数) 登录失败次数 + 失败次数。|
|successfulSignInCount|Int64|Active Directory 联合身份验证服务上成功登录的数量。|
|totalSignInCount|Int64|指定时段内 Active Directory 联合身份验证服务的成功登录数 + 登录失败次数。|
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


