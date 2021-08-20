---
title: authenticationMethodTarget 资源类型
description: 启用以将身份验证方法用作身份验证方法策略一部分的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 25f983d9f2f98474189bc286b4e13c9de897cc3a
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336696"
---
# <a name="authenticationmethodtarget-resource-type"></a>authenticationMethodTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

启用以将身份验证方法用作 Azure AD 中的身份验证方法策略一部分的用户或组的集合。 继承自 [实体](entity.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象标识符。|
|isRegistrationRequired|布尔值|确定是否强制用户注册身份验证方法。|
|targetType|authenticationMethodTargetType| 可能的值是 `user` ：、 `group` 和 `unknownFutureValue` 。|
|useForSignIn|布尔值|确定是否可以使用身份验证方法登录到 Azure AD。|

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
