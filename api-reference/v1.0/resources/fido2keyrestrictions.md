---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制执行的关键限制。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1781e39952bb3bf7cfb307d06ca3167ff58a2a6
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469449"
---
# <a name="fido2keyrestrictions-resource-type"></a>fido2KeyRestrictions 资源类型

命名空间：microsoft.graph

表示作为 [FIDO2](../resources/fido2authenticationmethodconfiguration.md)安全密钥身份验证方法策略的一部分强制执行的关键限制。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|aaGuids|String collection|Authenticator 证明 GUID 的集合。 AADGUIDs 定义密钥类型和制造商。|
|enforcementType|fido2RestrictionEnforcementType|强制类型。 可取值为：`allow`、`block`。|
|isEnforced|Boolean|确定是否启用配置的密钥强制。|

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
