---
title: 更新 secureScoreControlProfiles
description: 更新中更改各种属性，如 assignedTo 或 tenantNote 任何集成的解决方案的可编辑 secureScoreControlProfiles 属性。
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642028"
---
# <a name="update-securescorecontrolprofiles"></a>更新 secureScoreControlProfiles

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新中更改各种属性，如**assignedTo**或**tenantNote**任何集成的解决方案的可编辑**secureScoreControlProfiles**属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |   SecurityEvents.ReadWrite.All。  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | SecurityEvents.ReadWrite.All。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| 授权  | Bearer {code}。必需。|
|Prefer | 返回 = 表示形式。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。 下表列出了可以为 secureScoreControlProfile 更新字段。 不包含在请求正文中的现有属性的值不会更改。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|assignedTo|String|分析师控件的名称分配给进行会审、 实施或修复。|
|tenantNote|String|分析师评论 （用于客户控件管理） 的控件。|
|controlStateUpdates| String|分析师驱动控件上的设置。 可取值为：`ignore`、`thirdParty`、`reviewed`。|


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选请求标头，则该方法返回`200 OK`响应代码和响应正文中的更新的[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a>响应

下面是成功响应的示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
