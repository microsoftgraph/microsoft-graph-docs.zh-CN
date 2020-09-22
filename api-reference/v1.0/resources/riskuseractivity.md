---
title: riskUserActivity 资源类型
description: riskUserActivity 检测
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2b20a5796f5e1266271cd29d0768aa52927062a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991871"
---
# <a name="riskuseractivity-resource-type"></a>riskUserActivity 资源类型

命名空间：microsoft.graph

表示 azure AD 用户的风险活动，由 Azure AD Identity Protection 确定。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|介绍|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskEventTypes|String collection|检测到的风险事件的类型。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.riskUserActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskUserActivity",
  "riskEventTypes": [
    "String"
  ],
  "detail": "String"
}
```


