---
title: authenticationMethodTarget 资源类型
description: 在身份验证方法策略中启用使用身份验证方法的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7112249f618bbda31eddeb07967d201c8b641075
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418266"
---
# <a name="authenticationmethodtarget-resource-type"></a>authenticationMethodTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

启用身份验证方法的用户或组的集合，作为 Azure AD 中的身份验证方法策略的一部分。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Azure AD 用户或组的对象 Id。|
|isRegistrationRequired|布尔|确定是否强制用户注册身份验证方法。|
|targetType|authenticationMethodTargetType|可取值为：`user`、`group`。|
|useForSignIn|布尔|确定身份验证方法是否可用于登录 Azure AD。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
