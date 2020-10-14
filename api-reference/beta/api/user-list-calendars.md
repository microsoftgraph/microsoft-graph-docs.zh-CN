---
title: 列出日历
description: '获取用户的所有日历（`/calendars` 导航属性），从默认日历组或特定日历组中获取日历。 '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c2a5fe99eb342f49dd82dc1414396cdbd9ec25d3
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460073"
---
# <a name="list-calendars"></a><span data-ttu-id="f1b06-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="f1b06-103">List calendars</span></span>

<span data-ttu-id="f1b06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1b06-105">获取用户的所有日历（`/calendars` 导航属性），从默认日历组或特定日历组中获取日历。</span><span class="sxs-lookup"><span data-stu-id="f1b06-105">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="f1b06-106">权限</span><span class="sxs-lookup"><span data-stu-id="f1b06-106">Permissions</span></span>
<span data-ttu-id="f1b06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b06-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1b06-109">Permission type</span></span>      | <span data-ttu-id="f1b06-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1b06-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1b06-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1b06-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1b06-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1b06-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f1b06-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1b06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1b06-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1b06-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f1b06-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1b06-115">Application</span></span> | <span data-ttu-id="f1b06-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1b06-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1b06-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1b06-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f1b06-118">用户的所有日历。</span><span class="sxs-lookup"><span data-stu-id="f1b06-118">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="f1b06-119">默认 [calendarGroup](../resources/calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="f1b06-119">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="f1b06-120">特定 [calendarGroup](../resources/calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="f1b06-120">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1b06-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f1b06-121">Optional query parameters</span></span>
<span data-ttu-id="f1b06-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f1b06-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1b06-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1b06-123">Request headers</span></span>
| <span data-ttu-id="f1b06-124">标头</span><span class="sxs-lookup"><span data-stu-id="f1b06-124">Header</span></span>       | <span data-ttu-id="f1b06-125">值</span><span class="sxs-lookup"><span data-stu-id="f1b06-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1b06-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1b06-126">Authorization</span></span>  | <span data-ttu-id="f1b06-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1b06-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1b06-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1b06-129">Content-Type</span></span>   | <span data-ttu-id="f1b06-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b06-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1b06-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1b06-131">Request body</span></span>
<span data-ttu-id="f1b06-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1b06-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1b06-133">响应</span><span class="sxs-lookup"><span data-stu-id="f1b06-133">Response</span></span>

<span data-ttu-id="f1b06-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f1b06-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1b06-135">示例</span><span class="sxs-lookup"><span data-stu-id="f1b06-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1b06-136">请求</span><span class="sxs-lookup"><span data-stu-id="f1b06-136">Request</span></span>
<span data-ttu-id="f1b06-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1b06-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1b06-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b06-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="f1b06-139">C#</span><span class="sxs-lookup"><span data-stu-id="f1b06-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1b06-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1b06-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1b06-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1b06-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1b06-142">响应</span><span class="sxs-lookup"><span data-stu-id="f1b06-142">Response</span></span>
<span data-ttu-id="f1b06-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1b06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "calendarGroupId":null,
            "isDefaultCalendar": true,
            "canShare":true,
            "canViewPrivateItems":true,
            "hexColor": "",
            "isShared":false,
            "isSharedWithMe":false,
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
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
