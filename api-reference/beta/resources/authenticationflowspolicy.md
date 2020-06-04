---
title: authenticationFlowsPolicy 资源类型
description: '表示在租户级别上自助服务注册体验的策略配置，允许外部用户请求注册以进行审批。 '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 263b92c081545fc3ce337d25b4813d85fe034940
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556398"
---
# <a name="authenticationflowspolicy-resource-type"></a>authenticationFlowsPolicy 资源类型


命名空间：microsoft.graph

表示在租户级别上[自助服务注册体验的策略配置](../resources/selfservicesignupauthenticationflowconfiguration.md)，允许外部用户请求注册以进行审批。 它包含有关 ID、显示名称和说明的信息，并指示是否为策略启用自助服务注册。

## <a name="properties"></a>属性
|属性|类型|说明|
|:-------|:---|:----------|
|id|字符串| 继承的属性。 身份验证流策略的 ID。 可选。 只读。
|displayName|String| 继承的属性。 策略的人可读名称。 此属性不是键。 可选。 只读。|
|说明|String|继承的属性。 策略说明。 此属性不是键。 可选。 只读。|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |包含可传达是否启用或禁用自助注册的[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md)设置。 此属性不是键。 可选。 只读。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```
