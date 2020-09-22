---
title: identitySecurityDefaultsEnforcementPolicy 资源类型
description: 表示 Azure Active Directory 安全性默认策略。 安全性默认值包含针对常见攻击进行保护的预先配置的安全设置。
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13c7fd24c7f7d96149821a8a4e506e32ae681c78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086695"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>identitySecurityDefaultsEnforcementPolicy 资源类型

命名空间：microsoft.graph

表示 Azure Active Directory [安全性默认](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 策略。 安全性默认值包含针对常见攻击进行保护的预先配置的安全设置。

继承自 [policyBase](../resources/policybase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Get](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | 读取 **identitySecurityDefaultsEnforcementPolicy** 对象的属性。 |
| [更新](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | 更新 **identitySecurityDefaultsEnforcementPolicy** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|此策略的说明。 只读。|
|displayName|String|此策略的显示名称。 只读。|
|id|String|此策略的标识符。 只读。|
|isEnabled|Boolean|如果设置为 true，则会为租户启用 Azure Active Directory 安全性默认设置。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "",
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

