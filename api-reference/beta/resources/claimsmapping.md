---
title: claimsMapping 资源类型
description: 从令牌中的将声明映射到 Azure Active Directory B2C 可识别和使用的声明。
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 31ec191527509c015ab201c1464509fce64e549fd5475a377efbff0808973a74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239677"
---
# <a name="claimsmapping-resource-type"></a>claimsMapping 资源类型

命名空间：microsoft.graph

自定义标识提供程序将 ID 令牌发送回 Azure AD B2C 后，Azure AD B2C 从令牌中的将声明映射到 Azure AD B2C 可识别和使用的声明。

## <a name="properties"></a>属性
|属性|类型|描述|
|:-------|:---|:----------|
|userId|字符串|为已登录用户提供唯一标识符的声明。 这是必需属性。|
|displayName|String|为用户提供显示名称或全名的声明。它是必需的属性。|
|givenName|字符串|提供用户名字的声明。|
|surname|字符串|提供用户姓氏的声明。|
|email|字符串|提供用户名电子邮件地址的声明。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.claimsMapping"
}
-->

``` json
{
  "userId": "String",
  "givenName": "String",
  "surname": "String",
  "email": "String",
  "displayName": "String"
  }
```


