---
title: identitySecurityDefaultsEnforcementPolicy 资源类型
description: 代表Azure Active Directory默认策略。 安全默认值包含预配置的安全设置，可抵御常见攻击。
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d2e3c4af8bbb7dbac35f2a28a4704010b6c6d50542d2c5de9bd1cad3cb443a90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238088"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>identitySecurityDefaultsEnforcementPolicy 资源类型

命名空间：microsoft.graph

代表Azure Active Directory[默认策略](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。 安全默认值包含预配置的安全设置，可抵御常见攻击。

继承自 [policyBase](../resources/policybase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Get](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | 读取 **identitySecurityDefaultsEnforcementPolicy 对象** 的属性。 |
| [更新](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | 更新 **identitySecurityDefaultsEnforcementPolicy** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|此策略的说明。 只读。|
|displayName|String|此策略的显示名称。 只读。|
|id|String|此策略的标识符。 只读。|
|isEnabled|Boolean|如果设置为 `true` ，Azure Active Directory租户启用安全默认值。|

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
