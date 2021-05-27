---
title: authenticationMethodsPolicy 资源类型
description: 定义身份验证方法以及允许使用这些方法登录并执行 MFA (多重) 。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fdf86929b4098d9fb62f1426883b55d95c669f32
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682880"
---
# <a name="authenticationmethodspolicy-resource-type"></a>authenticationMethodsPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义身份验证方法以及允许使用它们登录和在 Azure AD) 中 (MFA) 执行Azure Active Directory (身份验证) 。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 authenticationMethodsPolicy](../api/authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。|
|[更新 authenticationMethodsPolicy](../api/authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|更新 [authenticationMethodsPolicy 对象](../resources/authenticationmethodspolicy.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略说明。|
|displayName|String|策略的名称。|
|id|String|策略的标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|上次更新策略的日期和时间。|
|policyVersion|String|使用的策略的版本。|
|registrationEnforcement|[registrationEnforcement](../resources/registrationenforcement.md)|在登录时强制注册。 此属性可用于提醒用户设置目标身份验证方法。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|authenticationMethodConfigurations|[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) 集合|表示每个身份验证方法的设置。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  } 
}
```
