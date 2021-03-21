---
title: keyValuePair 资源类型
description: 操作参数的键值对。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8897ea3d3788ce3fa846d845cb0854101b0b2ce7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960423"
---
# <a name="keyvaluepair-resource-type"></a>keyValuePair 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

操作参数的键值对。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|name|String|此键值对的名称。 可能的名称包括 `AdditionalWSFedEndpointCheckResult` `AllowedAuthenticationClassReferencesCheckResult` `AlwaysRequireAuthenticationCheckResult` ：、、、、、、、、、、。 `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult` `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult` `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult` `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult`|
|value|String|此键值对的值。 如果验证检查通过 () ， (验证检查失败) ， (验证检查为警告) ，则可能会返回结果 `0` `1` `2` 值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

