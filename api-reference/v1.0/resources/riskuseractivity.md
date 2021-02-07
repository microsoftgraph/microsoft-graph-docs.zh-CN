---
title: riskUserActivity 资源类型
description: riskUserActivity 检测
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7677832b2887bbb5dcddbeda21481da39f079669
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133222"
---
# <a name="riskuseractivity-resource-type"></a>riskUserActivity 资源类型

命名空间：microsoft.graph

表示 Azure AD 用户的风险活动，由 Azure AD Identity Protection 确定。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|detail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
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


