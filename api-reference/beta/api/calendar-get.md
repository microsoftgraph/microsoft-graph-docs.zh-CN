---
title: 获取日历
description: '获取 calendar 对象的属性和关系。 相应日历可以是用户的日历， '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed1d2dcc093d2c8180ea93afd8bf0758827890bf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438921"
---
# <a name="get-calendar"></a><span data-ttu-id="b16cf-104">获取日历</span><span class="sxs-lookup"><span data-stu-id="b16cf-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b16cf-105">获取 [calendar](../resources/calendar.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b16cf-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="b16cf-106">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="b16cf-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="b16cf-107">在下列两种情况下，应用可获取其他用户的日历：</span><span class="sxs-lookup"><span data-stu-id="b16cf-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="b16cf-108">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="b16cf-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b16cf-109">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b16cf-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b16cf-110">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="b16cf-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="b16cf-111">权限</span><span class="sxs-lookup"><span data-stu-id="b16cf-111">Permissions</span></span>
<span data-ttu-id="b16cf-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b16cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b16cf-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b16cf-114">Permission type</span></span>      | <span data-ttu-id="b16cf-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b16cf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b16cf-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b16cf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b16cf-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b16cf-117">Calendars.Read</span></span>    |
|<span data-ttu-id="b16cf-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b16cf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b16cf-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b16cf-119">Calendars.Read</span></span>    |
|<span data-ttu-id="b16cf-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b16cf-120">Application</span></span> | <span data-ttu-id="b16cf-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b16cf-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b16cf-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b16cf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b16cf-123">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b16cf-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="b16cf-124">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b16cf-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="b16cf-125">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b16cf-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b16cf-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b16cf-126">Optional query parameters</span></span>
<span data-ttu-id="b16cf-127">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b16cf-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b16cf-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b16cf-128">Request headers</span></span>
| <span data-ttu-id="b16cf-129">名称</span><span class="sxs-lookup"><span data-stu-id="b16cf-129">Name</span></span>       | <span data-ttu-id="b16cf-130">类型</span><span class="sxs-lookup"><span data-stu-id="b16cf-130">Type</span></span> | <span data-ttu-id="b16cf-131">说明</span><span class="sxs-lookup"><span data-stu-id="b16cf-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b16cf-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b16cf-132">Authorization</span></span>  | <span data-ttu-id="b16cf-133">string</span><span class="sxs-lookup"><span data-stu-id="b16cf-133">string</span></span>  | <span data-ttu-id="b16cf-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b16cf-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b16cf-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="b16cf-136">Request body</span></span>
<span data-ttu-id="b16cf-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b16cf-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b16cf-138">响应</span><span class="sxs-lookup"><span data-stu-id="b16cf-138">Response</span></span>

<span data-ttu-id="b16cf-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b16cf-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b16cf-140">示例</span><span class="sxs-lookup"><span data-stu-id="b16cf-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b16cf-141">请求</span><span class="sxs-lookup"><span data-stu-id="b16cf-141">Request</span></span>
<span data-ttu-id="b16cf-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b16cf-142">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b16cf-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b16cf-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b16cf-144">C#</span><span class="sxs-lookup"><span data-stu-id="b16cf-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b16cf-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="b16cf-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b16cf-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="b16cf-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b16cf-147">响应</span><span class="sxs-lookup"><span data-stu-id="b16cf-147">Response</span></span>
<span data-ttu-id="b16cf-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b16cf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
