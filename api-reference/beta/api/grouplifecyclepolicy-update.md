---
title: 更新 groupLifecyclePolicy
description: 更新 groupLifecyclePolicy 资源类型对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 69073693203981debbfa8010468df271ea65cef3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501761"
---
# <a name="update-grouplifecyclepolicy"></a>更新 groupLifecyclePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [groupLifecyclePolicy 资源类型](../resources/grouplifecyclepolicy.md)对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。
 

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持 |
|应用 | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称 | 说明 |
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|alternateNotificationEmails|字符串| 针对没有所有者的组向其发送通知的电子邮件地址列表。 可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。 |
|groupLifetimeInDays|Int32| 还剩多少天组就到期且需要续订。 续订后，组的有效期就会延长定义的天数。 |
|managedGroupTypes|String| 到期策略适用的组类型。 可取值为 **All**、**Selected** 或 **None**。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。
## <a name="example"></a>示例

##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a>响应
注意：为简洁起见，可能会截断此处展示的响应对象。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
