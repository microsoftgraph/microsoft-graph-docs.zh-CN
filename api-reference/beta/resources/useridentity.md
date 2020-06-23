---
title: userIdentity 类型
description: 表示访问评审的审阅者的 Azure AD 用户标识。
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1ab0a102cf430a98a0a5662af30cdd8cd36a3430
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846060"
---
# <a name="useridentity-type"></a>userIdentity 类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对于 Azure AD[访问审核](accessreviews-root.md)，此类型表示访问评审的创建者或审阅者的 Azure ad 用户标识。
在 Azure AD 审核日志的上下文中，这表示已启动或受审核活动影响的用户信息。

此类型继承自[标识](identity.md)，并且具有一个附加属性（用户的用户主体名称）。

## <a name="methods"></a>Methods

无。  [创建 accessReview](../api/accessreview-create.md)时，您可以在请求的正文中包含此类型的对象。

## <a name="properties"></a>属性

| 属性 | 类型 | Description|
|:---------------|:--------|:----------|
| `displayName` | `String` | 此身份的显示名称。 请注意，这可能并不总是可用，也不是最新的。    |
| `id`          | `String` | 身份的唯一标识符。  |
| `ipAddress`| `String`| 指示执行活动的用户使用的客户端 IP 地址（仅限审核日志）。|
| `userPrincipalName`|`String` | 用户的 userPrincipalName 属性。 |

## <a name="remarks"></a>注解

In some circumstances, the unique identifier for the actor may not be available.
In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.

## <a name="relationships"></a>关系

无。

## <a name="see-also"></a>另请参阅

| 方法                                                                | 返回类型                                | 说明                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [获取 accessReview 审阅者](../api/accessreview-listreviewers.md)    | [userIdentity](useridentity.md)集合 | 获取 accessReview 的审阅者。   |
| [添加 accessReview 审阅者](../api/accessreview-addreviewer.md)       | 无。                                      | 向 accessReview 添加审阅者。      |
| [删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。                                      | 从 accessReview 中删除审阅者。 |

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
