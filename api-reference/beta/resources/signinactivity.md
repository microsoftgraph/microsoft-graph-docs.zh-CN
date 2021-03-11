---
title: signInActivity 资源类型
description: 为特定用户提供上次登录日期。
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e48d2e64c71e67c623582552224a11636c7c6c7c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721857"
---
# <a name="signinactivity-resource-type"></a>signInActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定用户提供上次登录 [日期](user.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|特定用户的上次交互式登录日期。 可以使用此字段计算用户最后一次使用交互式身份验证方法登录到目录的时间。 此字段可用于生成报告，例如非活动用户。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为： `'2014-01-01T00:00:00Z'` 。 有关使用此属性的值有关详细信息，请参阅在 Azure AD 中管理 [非活动用户帐户](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)。|
|lastSignInRequestId|String|此用户执行的最后一次登录的请求 ID。|

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
  "lastSignInRequestId": "String"
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
