---
title: sessionlifetimepolicy 资源类型
description: 描述应用于Azure AD事件的会话生存期策略。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9da2ea66c726d48fa3b0a34c168debd16dbd8713
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137253"
---
# <a name="sessionlifetimepolicy-resource-type"></a>sessionlifetimepolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述应用于Azure AD事件的会话生存期策略。 

有关在会话中使用条件访问的会话Azure AD，请参阅条件[访问会话管理文档](/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime)。 

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|expirationRequirement|expirationRequirement|如果条件访问会话管理策略要求用户在此登录事件进行身份验证，则此字段描述需要身份验证的策略类型。 可取值包括：`rememberMultifactorAuthenticationOnTrustedDevices`、`tenantTokenLifetimePolicy`、`audienceTokenLifetimePolicy`、`signInFrequencyPeriodicReauthentication`、`ngcMfa`、`signInFrequencyEveryTime`、`unknownFutureValue`。|
|detail|String|应用于登录的条件访问会话管理策略的可读详细信息。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sessionLifetimePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sessionLifetimePolicy",
  "expirationRequirement": "String",
  "detail": "String"
}
```

