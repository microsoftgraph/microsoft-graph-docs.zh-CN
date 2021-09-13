---
title: authenticationMethodsPolicy 资源类型
description: 定义身份验证方法以及允许使用这些方法登录并执行 MFA (多重) 。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9abab0af31a67465db9989b42186759b12f746bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126959"
---
# <a name="authenticationmethodspolicy-resource-type"></a>authenticationMethodsPolicy 资源类型

命名空间：microsoft.graph

定义身份验证方法以及允许使用它们登录并执行 (Azure AD) 中的多重Azure Active Directory (身份验证) 。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 authenticationMethodsPolicy](../api/authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。|
|[更新 authenticationMethodsPolicy](../api/authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|更新 [authenticationMethodsPolicy 对象](../resources/authenticationmethodspolicy.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略说明。 只读。|
|displayName|String|策略的名称。 只读。|
|id|String|策略的标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|上次更新策略的日期和时间。 只读。|
|policyVersion|String|使用的策略的版本。 只读。|

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
}
```
