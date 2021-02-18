---
title: userIdentity 资源类型
description: 在 Azure AD 审核日志中，这表示启动或受审核活动影响的用户信息。
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 814b7106bf738711099d6d6e8d5e821b7b638318
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292159"
---
# <a name="useridentity-resource-type"></a>userIdentity 资源类型

命名空间：microsoft.graph

在 Azure AD 审核日志中，这表示启动或受审核活动影响的用户信息。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| displayName | String | 此身份的显示名称。 请注意，这可能并不总是可用或最新的。    |
| id          | String | 身份的唯一标识符。  |
| ipAddress   | String| 指示仅与用户一起执行活动 (审核日志使用的) 。|
| userPrincipalName | String  | 用户的 userPrincipalName 属性。 |

>**注意：** 在某些情况下，唯一标识符可能不可用。 在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

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
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

