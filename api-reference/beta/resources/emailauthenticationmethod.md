---
title: emailAuthenticationMethod 资源类型
description: 向用户注册的电子邮件地址的表示形式。 电子邮件是一种身份验证方法，仅提供 (SSPR) 的自助密码重置功能
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6dde3c9a859f2527241b66c0172d6b5dd877aac4
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418265"
---
# <a name="emailauthenticationmethod-resource-type"></a>emailAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户注册的电子邮件地址的表示形式。 电子邮件是一种身份验证方法，仅可用于 (SSPR) 的自助密码重置。 用户可能只有一种电子邮件身份验证方法。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List](../api/emailauthenticationmethod-list.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 集合|检索用户的 emailAuthenticationMethods 的列表。 用户可能只有一种电子邮件身份验证方法。|
|[创建](../api/emailauthenticationmethod-post.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|创建用户的 emailMethods 对象。|
|[获取](../api/emailauthenticationmethod-get.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|检索用户的 emailAuthenticationMethod 对象的属性。|
|[更新](../api/emailauthenticationmethod-update.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|更新用户的 emailMethods 对象的属性。|
|[删除](../api/emailauthenticationmethod-delete.md)|无|删除用户的 emailAuthenticationMethod 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|向此用户注册的电子邮件地址的标识符。|
|emailAddress|String|向此用户注册的电子邮件地址。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

