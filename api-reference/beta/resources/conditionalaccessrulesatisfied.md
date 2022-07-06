---
title: conditionalAccessRulesSatisfied 资源类型
description: 指示在身份验证事件中满足的条件访问规则。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 50ebb20c38275a7ab0192b56ca67058ff640948f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645437"
---
# <a name="conditionalaccessrulessatisfied-resource-type"></a>conditionalAccessRulesSatisfied 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示与相应登录活动触发的已应用条件访问策略或策略相关的属性。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|conditionalAccessCondition|conditionalAccessConditions|指满足的条件访问策略条件。 可能的值是：`none`、、`application`、`devicePlatform``users`、`location`、`clientType`、`signInRisk`、`userRisk`、`time``deviceState`、`client`、`ipAddressSeenByAzureAD`、`ipAddressSeenByResourceProvider`、`unknownFutureValue`、、 `servicePrincipals``servicePrincipalRisk` 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的以下值： `servicePrincipals``servicePrincipalRisk`|
|ruleSatisfied|conditionalAccessRule|指满足的条件访问策略条件。 可能的值为：`allApps`、`firstPartyApps`、、`office365`、`acr``appId`、`appFilter`、`allUsers`、`guest`、、`roleId``groupId`、`userId``devicePlatform``allLocations``allDevicePlatforms``allTrustedLocations``insideCorpnet`、、`locationId`、`allDevices`、、 `serviceProvider``b2bDirectConnectUser``otherExternalUser``deviceFilter``deviceState``unknownFutureValue``deviceFilterIncludeRuleNotMatched``allDeviceStates``anonymizedIPAddress``unfamiliarFeatures``nationStateIPAddress``realTimeThreatIntelligence``internalGuest``b2bCollaborationGuest``b2bCollaborationMember` 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的以下值： `deviceFilterIncludeRuleNotMatched``allDeviceStates`|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRuleSatisfied",
  "conditionalAccessCondition": "String",
  "ruleSatisfied": "String"
}
```
