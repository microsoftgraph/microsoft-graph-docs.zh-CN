---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制执行的关键限制。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a40a185f688038d3c849113ae8e9b53c4f0652f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133796"
---
# <a name="fido2keyrestrictions-resource-type"></a>fido2KeyRestrictions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示作为 FIDO2 安全密钥身份验证方法策略的一部分 [强制执行的关键限制](../resources/fido2authenticationmethodconfiguration.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|aaGuids|字符串集合|Authenticator 证明 GUID 的集合。 AADGUID 定义密钥类型和制造商。|
|enforcementType|fido2RestrictionEnforcementType|强制类型。 可取值为：`allow`、`block`。|
|isEnforced|Boolean|确定是否启用已配置的密钥强制。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
