---
title: Update calendar
description: '更新 calendar 对象的属性。 相应日历可以是用户的日历， '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 63ac3812bcf71418f8747502d6212be18d55dbaf
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897825"
---
# <a name="update-calendar"></a><span data-ttu-id="a37fb-104">更新日历</span><span class="sxs-lookup"><span data-stu-id="a37fb-104">Update calendar</span></span>

<span data-ttu-id="a37fb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a37fb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a37fb-106">更新 [calendar](../resources/calendar.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a37fb-106">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="a37fb-107">日历可以是[用户](../resources/user.md)的一个，也可以是 Microsoft 365[组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="a37fb-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a37fb-108">权限</span><span class="sxs-lookup"><span data-stu-id="a37fb-108">Permissions</span></span>
<span data-ttu-id="a37fb-109">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a37fb-109">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="a37fb-110">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a37fb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a37fb-111">日历</span><span class="sxs-lookup"><span data-stu-id="a37fb-111">Calendar</span></span> | <span data-ttu-id="a37fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a37fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a37fb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a37fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a37fb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a37fb-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="a37fb-115">用户日历</span><span class="sxs-lookup"><span data-stu-id="a37fb-115">user calendar</span></span> | <span data-ttu-id="a37fb-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a37fb-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="a37fb-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a37fb-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="a37fb-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a37fb-118">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="a37fb-119">组日历</span><span class="sxs-lookup"><span data-stu-id="a37fb-119">group calendar</span></span> | <span data-ttu-id="a37fb-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a37fb-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="a37fb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a37fb-121">Not supported.</span></span> | <span data-ttu-id="a37fb-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="a37fb-122">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a37fb-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a37fb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a37fb-124">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="a37fb-124">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="a37fb-125">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="a37fb-125">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="a37fb-126">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="a37fb-126">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a37fb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="a37fb-127">Request headers</span></span>
| <span data-ttu-id="a37fb-128">标头</span><span class="sxs-lookup"><span data-stu-id="a37fb-128">Header</span></span>       | <span data-ttu-id="a37fb-129">值</span><span class="sxs-lookup"><span data-stu-id="a37fb-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a37fb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a37fb-130">Authorization</span></span>  | <span data-ttu-id="a37fb-131">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a37fb-131">Bearer {token}.</span></span> <span data-ttu-id="a37fb-132">Required.</span><span class="sxs-lookup"><span data-stu-id="a37fb-132">Required.</span></span>  |
| <span data-ttu-id="a37fb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a37fb-133">Content-Type</span></span>  | <span data-ttu-id="a37fb-134">application/json.</span><span class="sxs-lookup"><span data-stu-id="a37fb-134">application/json.</span></span> <span data-ttu-id="a37fb-135">Required.</span><span class="sxs-lookup"><span data-stu-id="a37fb-135">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a37fb-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a37fb-136">Request body</span></span>
<span data-ttu-id="a37fb-137">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="a37fb-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a37fb-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="a37fb-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a37fb-139">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="a37fb-139">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a37fb-140">属性</span><span class="sxs-lookup"><span data-stu-id="a37fb-140">Property</span></span>     | <span data-ttu-id="a37fb-141">类型</span><span class="sxs-lookup"><span data-stu-id="a37fb-141">Type</span></span>   |<span data-ttu-id="a37fb-142">说明</span><span class="sxs-lookup"><span data-stu-id="a37fb-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a37fb-143">color</span><span class="sxs-lookup"><span data-stu-id="a37fb-143">color</span></span>|<span data-ttu-id="a37fb-144">String</span><span class="sxs-lookup"><span data-stu-id="a37fb-144">String</span></span>|<span data-ttu-id="a37fb-145">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span><span class="sxs-lookup"><span data-stu-id="a37fb-145">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span></span> <span data-ttu-id="a37fb-146">The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="a37fb-146">The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="a37fb-147">name</span><span class="sxs-lookup"><span data-stu-id="a37fb-147">name</span></span>|<span data-ttu-id="a37fb-148">String</span><span class="sxs-lookup"><span data-stu-id="a37fb-148">String</span></span>|<span data-ttu-id="a37fb-149">日历名称。</span><span class="sxs-lookup"><span data-stu-id="a37fb-149">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="a37fb-150">响应</span><span class="sxs-lookup"><span data-stu-id="a37fb-150">Response</span></span>

<span data-ttu-id="a37fb-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a37fb-151">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a37fb-152">示例</span><span class="sxs-lookup"><span data-stu-id="a37fb-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="a37fb-153">请求</span><span class="sxs-lookup"><span data-stu-id="a37fb-153">Request</span></span>
<span data-ttu-id="a37fb-154">下面的示例更新已登录用户的默认日历的名称。</span><span class="sxs-lookup"><span data-stu-id="a37fb-154">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="a37fb-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="a37fb-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
# <a name="c"></a>[<span data-ttu-id="a37fb-156">C#</span><span class="sxs-lookup"><span data-stu-id="a37fb-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a37fb-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a37fb-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a37fb-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a37fb-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a37fb-159">Java</span><span class="sxs-lookup"><span data-stu-id="a37fb-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a37fb-160">响应</span><span class="sxs-lookup"><span data-stu-id="a37fb-160">Response</span></span>
<span data-ttu-id="a37fb-161">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a37fb-161">Here is an example of the response.</span></span> <span data-ttu-id="a37fb-162">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a37fb-162">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a37fb-163">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a37fb-163">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
