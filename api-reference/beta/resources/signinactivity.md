---
title: signInActivity 资源类型
description: 为特定用户提供最后一次交互式或非交互式登录时间。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c67966902315f4b8ef4ab75f7f0c8d3cb5988f98
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604180"
---
# <a name="signinactivity-resource-type"></a>signInActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定用户提供最后一次交互式或非交互式登录 [时间](user.md)。 由于 signInActivity 描述了用户对象的属性，Azure AD只要用户对象存在，就存储用户的登录活动。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|特定用户的上次交互式登录日期和时间。 可以使用此字段计算用户最后一次使用交互式身份验证方法登录到目录的时间。 此字段可用于生成报告，例如非活动用户。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` ：。 Azure AD维护返回到 2020 年 4 月的交互式登录。 有关使用此属性的值的信息，请参阅管理非活动用户帐户[Azure AD。](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
|lastSignInRequestId|String|此用户执行的最后一次交互式登录的请求标识符。|
|lastNonInteractiveSignInDateTime|DateTimeOffset|特定用户的上一个非交互式登录日期。 可以使用此字段计算客户端最后一次代表用户登录到目录的时间。 由于某些用户可能会使用客户端访问租户资源，而不是直接登录租户，因此可以使用非交互式登录日期和 lastSignInDateTime 来标识非活动用户。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` ：。 Azure AD维护到 2020 年 5 月的非交互式登录。 有关使用此属性的值的信息，请参阅管理非活动用户帐户[Azure AD。](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
|lastNonInteractiveSignInRequestId|String|此用户执行的最后一个非交互式登录的请求标识符。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String",
  "lastNonInteractiveSignInDateTime": "String (timestamp)",
  "lastNonInteractiveSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
