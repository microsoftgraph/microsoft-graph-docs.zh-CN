---
title: conditionalAccessRulesSatisfied 资源类型
description: 指示身份验证事件期间满足的条件访问规则。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c86ffeaa52941d863529ed4ed3a72d7216359480
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647056"
---
# <a name="conditionalaccessrulessatisfied-resource-type"></a>conditionalAccessRulesSatisfied 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示与由相应登录活动触发的已应用的条件访问策略相关的属性。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|conditionalAccessCondition|conditionalAccessConditions|引用满足的条件访问策略条件。 可能的值是 `none` `application` `users` `devicePlatform` `location` `clientType` ：、、、、、、 `signInRisk` `userRisk` `time` `deviceState` `client` `ipAddressSeenByAzureAD` `ipAddressSeenByResourceProvider` `unknownFutureValue` `servicePrincipals` `servicePrincipalRisk` 。 请注意，必须使用请求标头获取此可发展枚举中的以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `servicePrincipals` `servicePrincipalRisk` ：、。|
|ruleSatisfied|conditionalAccessRule|引用满足的条件访问策略条件。 可能的值包括 `allApps` `firstPartyApps` `office365` `appId` `acr` `appFilter` ：、、、 `allUsers` `guest` `groupId` `roleId` `userId` `allDevicePlatforms` `devicePlatform` `allLocations` `insideCorpnet` `allTrustedLocations` `locationId` `allDevices` `deviceFilter` `deviceState` `unknownFutureValue` `deviceFilterIncludeRuleNotMatched` `allDeviceStates` 。 请注意，必须使用请求标头获取此可发展枚举中的以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `deviceFilterIncludeRuleNotMatched` `allDeviceStates` ：、。|


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
