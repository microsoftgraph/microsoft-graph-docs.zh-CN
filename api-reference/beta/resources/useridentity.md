---
title: userIdentity 类型
description: 表示访问评审的审阅者的 Azure AD 用户标识。
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e42f862cfbb82982ce91a0ed7339f19f9469037b
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698252"
---
# <a name="useridentity-type"></a>userIdentity 类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对于 Azure AD [访问评审](accessreviews-root.md)，此类型表示访问评审的创建者或审阅者的 Azure AD 用户标识。
在 Azure AD 审核日志的上下文中，这表示发起或受审核活动影响的用户信息。

此类型继承自 [标识](identity.md) ，并具有一个附加属性，即用户的用户主体名称。

## <a name="methods"></a>方法

无。  [创建 accessReview](../api/accessreview-create.md) 时，将在请求正文中包含此类对象。

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| displayName       | String | 此身份的显示名称。 请注意，这可能并不总是可用或最新。 |
| id                | String | 身份的唯一标识符。 可为 Null。                                                   |
| ipAddress         | String | 指示执行活动的用户使用的客户端 IP 地址 (仅) 审核日志。 |
| userPrincipalName | 字符串 | 用户的 userPrincipalName 属性。                                           |

### <a name="remarks"></a>注解

在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

## <a name="relationships"></a>关系

无。

## <a name="see-also"></a>另请参阅

| 方法                                                                | 返回类型                                | 说明                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [获取 accessReview 审阅者](../api/accessreview-listreviewers.md)    | [userIdentity](useridentity.md) 集合 | 获取 accessReview 的审阅者。   |
| [添加 accessReview 审阅器](../api/accessreview-addreviewer.md)       | 无。                                      | 将审阅者添加到 accessReview。      |
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


