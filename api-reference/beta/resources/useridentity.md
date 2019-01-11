---
title: userIdentity 类型
description: '为 Azure AD 访问 reviews （英文），此类型的访问评审的审阅者表示 Azure AD 用户标识。  '
localization_priority: Normal
ms.openlocfilehash: 5b629fff4c5cecd513777cc5004646aac5f1c85b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839639"
---
# <a name="useridentity-type"></a>userIdentity 类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

对于[access 会检查](accessreviews-root.md)Azure AD，此类型的访问评审的审阅者代表 Azure AD 用户标识。  
在 Azure AD 审核日志的上下文中，这表示启动或审核活动受影响的用户信息。

此类型继承自[identity](identity.md)和一个其他属性，用户的用户主体名称。

## <a name="methods"></a>方法

无。  您将在请求正文中包含此类型的对象时[创建 accessReview](../api/accessreview-create.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
| `displayName` | `String` | 标识的显示名称。 请注意，这可能会始终不可用或最新。    |
| `id`          | `String` | 身份的唯一标识符。  |
| `ipAddress`| `String`| 指示执行活动 （仅用于审核日志） 的用户所使用的客户端 IP 地址。|
| `userPrincipalName`|`String` | 用户的 userPrincipalName 属性。 |

## <a name="remarks"></a>注解

在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

## <a name="relationships"></a>Relationships

无。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview 审阅者](../api/accessreview-listreviewers.md) |       [userIdentity](useridentity.md)集合| 要获取 accessReview 审阅的者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   将审阅者添加到 accessReview。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   删除 accessReview 审阅者。 |

## <a name="json-representation"></a>JSON 表示形式

下面是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
