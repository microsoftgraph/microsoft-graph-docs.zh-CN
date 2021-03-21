---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制执行的关键限制。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fd319b64d124fc2c80c7f851a2e062d3568c2d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964683"
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
