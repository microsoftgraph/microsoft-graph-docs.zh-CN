---
title: authenticationMethodTarget 资源类型
description: 启用以将身份验证方法用作身份验证方法策略一部分的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f75a0ee81f1c43923a910bd86df4828c276706e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469106"
---
# <a name="authenticationmethodtarget-resource-type"></a>authenticationMethodTarget 资源类型

命名空间：microsoft.graph

启用以将身份验证方法用作 Azure AD 中身份验证方法策略一部分的用户或组的集合。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象 ID。|
|isRegistrationRequired|Boolean|确定是否强制用户注册身份验证方法。|
|targetType|authenticationMethodTargetType|可取值为：`user`、`group`。|
|useForSignIn|Boolean|确定是否可以使用身份验证方法登录到 Azure AD。|

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
