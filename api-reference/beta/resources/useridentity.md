---
title: userIdentity 类型
description: '对于 azure ad 访问审核, 此类型表示访问审核的审阅者的 Azure ad 用户标识。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 554aa9d38b4635ab3410fd95441b5c5045a1f1f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345045"
---
# <a name="useridentity-type"></a>userIdentity 类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对于 azure ad[访问审核](accessreviews-root.md), 此类型表示访问评审的创建者或审阅者的 Azure ad 用户标识。  
在 Azure AD 审核日志的上下文中, 这表示已启动或受审核活动影响的用户信息。

此类型继承自[标识](identity.md), 并且具有一个附加属性 (用户的用户主体名称)。

## <a name="methods"></a>方法

无。  [创建 accessReview](../api/accessreview-create.md)时, 您可以在请求的正文中包含此类型的对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `displayName` | `String` | 此身份的显示名称。 请注意, 这可能并不总是可用, 也不是最新的。    |
| `id`          | `String` | 身份的唯一标识符。  |
| `ipAddress`| `String`| 指示执行活动的用户使用的客户端 IP 地址 (仅限审核日志)。|
| `userPrincipalName`|`String` | 用户的 userPrincipalName 属性。 |

## <a name="remarks"></a>注解

在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

## <a name="relationships"></a>Relationships

无。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview 审阅者](../api/accessreview-listreviewers.md) |       [userIdentity](useridentity.md)集合| 获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   向 accessReview 添加审阅者。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   从 accessReview 中删除审阅者。 |

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
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
