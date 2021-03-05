---
title: identitySecurityDefaultsEnforcementPolicy 资源类型
description: 代表 Azure Active Directory 安全默认策略。 安全默认设置包含防止常见攻击的预配置安全设置。
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 21b012338e6ca168e932a8aaf2560ce825304ae9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439840"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>identitySecurityDefaultsEnforcementPolicy 资源类型

命名空间：microsoft.graph

代表 Azure Active Directory [安全默认](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 策略。 安全默认设置包含防止常见攻击的预配置安全设置。

继承自 [policyBase](../resources/policybase.md)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | 读取 **identitySecurityDefaultsEnforcementPolicy 对象** 的属性。 |
| [更新](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | 更新 **identitySecurityDefaultsEnforcementPolicy** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|此策略的说明。 只读。|
|displayName|String|此策略的显示名称。 只读。|
|id|String|此策略的标识符。 只读。|
|isEnabled|Boolean|如果设置为 true，则为租户启用 Azure Active Directory 安全默认值。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySecurityDefaultsEnforcementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
