---
title: 获取日历
description: '获取 calendar 对象的属性和关系。 相应日历可以是用户的日历， '
ms.localizationpriority: high
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c782b4d259f6926c7066e9cdfc956e7db430622a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125445"
---
# <a name="get-calendar"></a>获取日历

命名空间：microsoft.graph

获取 [calendar](../resources/calendar.md) 对象的属性和关系。 可以是[用户](../resources/user.md)的日历，也可以是 Microsoft 365 [组](../resources/group.md)的默认日历。

在下列两种情况下，应用可获取其他用户的日历：

* 如果该应用具有应用程序权限，或者
* 如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。 请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。

## <a name="permissions"></a>权限
根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。 要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。

| 日历 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
| 用户日历 | Calendars.Read、Calendars.ReadWrite | Calendars.Read、Calendars.ReadWrite | Calendars.Read、Calendars.ReadWrite |
| 组日历 | Group.Read.All、Group.ReadWrite.All | 不支持。 | 不支持。 |


## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
用户或组的默认 [日历](../resources/calendar.md)。
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}
```
指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。
## <a name="example"></a>示例
### <a name="request"></a>请求
下面的示例提供了登录用户的默认日历。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "canEdit":true,
    "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
