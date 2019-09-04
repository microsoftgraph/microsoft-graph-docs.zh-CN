---
title: 获取日历
description: '获取 calendar 对象的属性和关系。 相应日历可以是用户的日历， '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e6200e50e5a4e8704d5f2b11321ddbd86ad9ac73
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718704"
---
# <a name="get-calendar"></a><span data-ttu-id="59736-104">获取日历</span><span class="sxs-lookup"><span data-stu-id="59736-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59736-105">获取 [calendar](../resources/calendar.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59736-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="59736-106">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="59736-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="59736-107">在下列两种情况下，应用可获取其他用户的日历：</span><span class="sxs-lookup"><span data-stu-id="59736-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="59736-108">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="59736-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="59736-109">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="59736-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="59736-110">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="59736-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="59736-111">权限</span><span class="sxs-lookup"><span data-stu-id="59736-111">Permissions</span></span>
<span data-ttu-id="59736-112">根据事件所在的日历类型和请求的权限类型 (委派或应用程序), 需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="59736-112">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="59736-113">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59736-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59736-114">日历</span><span class="sxs-lookup"><span data-stu-id="59736-114">Calendar</span></span> | <span data-ttu-id="59736-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59736-115">Delegated (work or school account)</span></span> | <span data-ttu-id="59736-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59736-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59736-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59736-117">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="59736-118">用户日历</span><span class="sxs-lookup"><span data-stu-id="59736-118">user calendar</span></span> | <span data-ttu-id="59736-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59736-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="59736-120">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59736-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="59736-121">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59736-121">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="59736-122">组 日历</span><span class="sxs-lookup"><span data-stu-id="59736-122">group calendar</span></span> | <span data-ttu-id="59736-123">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59736-123">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="59736-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="59736-124">Not supported.</span></span> | <span data-ttu-id="59736-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="59736-125">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="59736-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59736-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="59736-127">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="59736-127">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="59736-128">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="59736-128">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="59736-129">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="59736-129">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59736-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59736-130">Optional query parameters</span></span>
<span data-ttu-id="59736-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59736-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59736-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="59736-132">Request headers</span></span>
| <span data-ttu-id="59736-133">名称</span><span class="sxs-lookup"><span data-stu-id="59736-133">Name</span></span>       | <span data-ttu-id="59736-134">类型</span><span class="sxs-lookup"><span data-stu-id="59736-134">Type</span></span> | <span data-ttu-id="59736-135">说明</span><span class="sxs-lookup"><span data-stu-id="59736-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59736-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="59736-136">Authorization</span></span>  | <span data-ttu-id="59736-137">string</span><span class="sxs-lookup"><span data-stu-id="59736-137">string</span></span>  | <span data-ttu-id="59736-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59736-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59736-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="59736-140">Request body</span></span>
<span data-ttu-id="59736-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59736-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59736-142">响应</span><span class="sxs-lookup"><span data-stu-id="59736-142">Response</span></span>

<span data-ttu-id="59736-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59736-143">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59736-144">示例</span><span class="sxs-lookup"><span data-stu-id="59736-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59736-145">请求</span><span class="sxs-lookup"><span data-stu-id="59736-145">Request</span></span>
<span data-ttu-id="59736-146">下面的示例获取已登录用户的默认日历。</span><span class="sxs-lookup"><span data-stu-id="59736-146">The following example gets the signed-in user's default calendar.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="59736-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="59736-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59736-148">C#</span><span class="sxs-lookup"><span data-stu-id="59736-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59736-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59736-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59736-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="59736-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59736-151">响应</span><span class="sxs-lookup"><span data-stu-id="59736-151">Response</span></span>
<span data-ttu-id="59736-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59736-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
