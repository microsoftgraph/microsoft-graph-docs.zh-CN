---
title: emailAuthenticationMethod 资源类型
description: '注册到用户的电子邮件地址的表示形式。 电子邮件是一种身份验证方法，仅适用于 SSPR (的自助服务密码) '
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a24a67fdb4bcc054036de26ba235bf4bac0f2da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440365"
---
# <a name="emailauthenticationmethod-resource-type"></a>emailAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

注册到用户的电子邮件地址的表示形式。 电子邮件是一种身份验证方法，仅适用于 SSPR (的自助服务密码) 。 用户可能只有一种电子邮件身份验证方法。


## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List](../api/emailauthenticationmethod-list.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 集合|检索用户的电子邮件AuthenticationMethods 的列表。 用户可能只有一种电子邮件身份验证方法。|
|[创建](../api/emailauthenticationmethod-post.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|创建用户的电子邮件Methods 对象。|
|[获取](../api/emailauthenticationmethod-get.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|检索用户 emailAuthenticationMethod 对象的属性。|
|[更新](../api/emailauthenticationmethod-update.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|更新用户 emailMethods 对象的属性。|
|[删除](../api/emailauthenticationmethod-delete.md)|无|删除用户的电子邮件AuthenticationMethod 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|注册到此用户的电子邮件地址的标识符。|
|emailAddress|String|注册到此用户的电子邮件地址。|

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

