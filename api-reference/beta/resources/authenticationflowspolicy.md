---
title: authenticationFlowsPolicy 资源类型
description: '表示租户级别的自助注册体验策略配置，允许外部用户请求注册以进行批准。 '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cc7f6261e4db4b908d6ab3e0ab3c41504ce8462b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232107"
---
# <a name="authenticationflowspolicy-resource-type"></a>authenticationFlowsPolicy 资源类型


命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户级别的[自助注册体验策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行批准。 它包含有关 ID、显示名称和说明的信息，并指示是否对该策略启用了自助注册。

## <a name="properties"></a>属性
|属性|类型|说明|
|:-------|:---|:----------|
|id|字符串| 继承的属性。 身份验证流策略的 ID。 可选。 只读。
|displayName|字符串| 继承的属性。 策略的用户可读名称。 此属性不是一个键。 可选。 只读。|
|说明|字符串|继承的属性。 策略说明。 此属性不是一个键。 可选。 只读。|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |包含用于传达是否已启用或禁用自助注册的 [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) 设置。 此属性不是一个键。 可选。 只读。 |

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


