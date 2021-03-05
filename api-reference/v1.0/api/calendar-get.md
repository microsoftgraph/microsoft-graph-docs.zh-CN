---
title: 获取日历
description: '获取 calendar 对象的属性和关系。 相应日历可以是用户的日历， '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7af1c3679ab9c6d4d75e8618acf17d653619b869
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434896"
---
# <a name="get-calendar"></a><span data-ttu-id="5a0ff-104">获取日历</span><span class="sxs-lookup"><span data-stu-id="5a0ff-104">Get calendar</span></span>

<span data-ttu-id="5a0ff-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a0ff-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a0ff-106">获取 [calendar](../resources/calendar.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-106">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="5a0ff-107">可以是[用户](../resources/user.md)的日历，也可以是 Microsoft 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="5a0ff-108">在下列两种情况下，应用可获取其他用户的日历：</span><span class="sxs-lookup"><span data-stu-id="5a0ff-108">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="5a0ff-109">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="5a0ff-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5a0ff-110">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5a0ff-111">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-111">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a0ff-112">权限</span><span class="sxs-lookup"><span data-stu-id="5a0ff-112">Permissions</span></span>
<span data-ttu-id="5a0ff-113">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-113">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="5a0ff-114">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a0ff-115">日历</span><span class="sxs-lookup"><span data-stu-id="5a0ff-115">Calendar</span></span> | <span data-ttu-id="5a0ff-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a0ff-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5a0ff-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a0ff-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a0ff-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a0ff-118">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="5a0ff-119">用户日历</span><span class="sxs-lookup"><span data-stu-id="5a0ff-119">user calendar</span></span> | <span data-ttu-id="5a0ff-120">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a0ff-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="5a0ff-121">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a0ff-121">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="5a0ff-122">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a0ff-122">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="5a0ff-123">组日历</span><span class="sxs-lookup"><span data-stu-id="5a0ff-123">group calendar</span></span> | <span data-ttu-id="5a0ff-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0ff-124">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="5a0ff-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-125">Not supported.</span></span> | <span data-ttu-id="5a0ff-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-126">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="5a0ff-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a0ff-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5a0ff-128">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-128">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="5a0ff-129">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-129">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}
```
<span data-ttu-id="5a0ff-130">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-130">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a0ff-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a0ff-131">Optional query parameters</span></span>
<span data-ttu-id="5a0ff-132">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5a0ff-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a0ff-133">Request headers</span></span>
| <span data-ttu-id="5a0ff-134">名称</span><span class="sxs-lookup"><span data-stu-id="5a0ff-134">Name</span></span>       | <span data-ttu-id="5a0ff-135">类型</span><span class="sxs-lookup"><span data-stu-id="5a0ff-135">Type</span></span> | <span data-ttu-id="5a0ff-136">说明</span><span class="sxs-lookup"><span data-stu-id="5a0ff-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5a0ff-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a0ff-137">Authorization</span></span>  | <span data-ttu-id="5a0ff-138">string</span><span class="sxs-lookup"><span data-stu-id="5a0ff-138">string</span></span>  | <span data-ttu-id="5a0ff-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a0ff-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a0ff-141">Request body</span></span>
<span data-ttu-id="5a0ff-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a0ff-143">响应</span><span class="sxs-lookup"><span data-stu-id="5a0ff-143">Response</span></span>

<span data-ttu-id="5a0ff-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-144">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a0ff-145">示例</span><span class="sxs-lookup"><span data-stu-id="5a0ff-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a0ff-146">请求</span><span class="sxs-lookup"><span data-stu-id="5a0ff-146">Request</span></span>
<span data-ttu-id="5a0ff-147">下面的示例提供了登录用户的默认日历。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-147">The following example gets the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a0ff-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a0ff-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="5a0ff-149">C#</span><span class="sxs-lookup"><span data-stu-id="5a0ff-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a0ff-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a0ff-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a0ff-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a0ff-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a0ff-152">Java</span><span class="sxs-lookup"><span data-stu-id="5a0ff-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5a0ff-153">响应</span><span class="sxs-lookup"><span data-stu-id="5a0ff-153">Response</span></span>
<span data-ttu-id="5a0ff-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a0ff-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
