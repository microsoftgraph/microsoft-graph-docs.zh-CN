---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制执行的关键限制。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37b9e2c7a66b3ce9a43c08560f5e5f4a8e0acc2e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036527"
---
# <a name="fido2keyrestrictions-resource-type"></a>fido2KeyRestrictions 资源类型

命名空间：microsoft.graph

表示作为 [FIDO2](../resources/fido2authenticationmethodconfiguration.md)安全密钥身份验证方法策略的一部分强制执行的关键限制。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|aaGuids|字符串集合|一组Authenticator证明 GUID。 AADGUIDs 定义密钥类型和制造商。|
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
