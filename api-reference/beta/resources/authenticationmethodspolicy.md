---
title: authenticationMethodsPolicy 资源类型
description: 定义身份验证方法以及允许使用这些方法登录并执行 MFA (多重) 。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 470e9cb94fc6145fde98aaa6e35a3b99aef66f8e
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239363"
---
# <a name="authenticationmethodspolicy-resource-type"></a>authenticationMethodsPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义身份验证方法以及允许使用它们登录并执行 MFA 中 MFA (多重) Azure Active Directory (Azure AD) 。

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
|authenticationMethodConfigurations|[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) 集合|表示每个身份验证方法的设置。 在 `GET /policies/authenticationMethodsPolicy` 时自动展开。|

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
