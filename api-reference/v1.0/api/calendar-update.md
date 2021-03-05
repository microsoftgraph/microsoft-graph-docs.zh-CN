---
title: Update calendar
description: '更新 calendar 对象的属性。 相应日历可以是用户的日历， '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 870432cf062fa1aa933a73f479fcfedf66b638e6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434858"
---
# <a name="update-calendar"></a><span data-ttu-id="04f28-104">更新日历</span><span class="sxs-lookup"><span data-stu-id="04f28-104">Update calendar</span></span>

<span data-ttu-id="04f28-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04f28-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04f28-106">更新 [calendar](../resources/calendar.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04f28-106">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="04f28-107">可以是[用户](../resources/user.md)的日历，也可以是 Microsoft 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="04f28-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="04f28-108">权限</span><span class="sxs-lookup"><span data-stu-id="04f28-108">Permissions</span></span>
<span data-ttu-id="04f28-109">根据事件所处日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="04f28-109">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="04f28-110">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04f28-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04f28-111">日历</span><span class="sxs-lookup"><span data-stu-id="04f28-111">Calendar</span></span> | <span data-ttu-id="04f28-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04f28-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04f28-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04f28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04f28-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="04f28-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="04f28-115">用户日历</span><span class="sxs-lookup"><span data-stu-id="04f28-115">user calendar</span></span> | <span data-ttu-id="04f28-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f28-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="04f28-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f28-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="04f28-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f28-118">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="04f28-119">组日历</span><span class="sxs-lookup"><span data-stu-id="04f28-119">group calendar</span></span> | <span data-ttu-id="04f28-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f28-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="04f28-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="04f28-121">Not supported.</span></span> | <span data-ttu-id="04f28-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="04f28-122">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="04f28-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04f28-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="04f28-124">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="04f28-124">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="04f28-125">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="04f28-125">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}
```
<span data-ttu-id="04f28-126">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="04f28-126">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="04f28-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="04f28-127">Request headers</span></span>
| <span data-ttu-id="04f28-128">标头</span><span class="sxs-lookup"><span data-stu-id="04f28-128">Header</span></span>       | <span data-ttu-id="04f28-129">值</span><span class="sxs-lookup"><span data-stu-id="04f28-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04f28-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f28-130">Authorization</span></span>  | <span data-ttu-id="04f28-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04f28-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04f28-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04f28-133">Content-Type</span></span>  | <span data-ttu-id="04f28-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="04f28-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04f28-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="04f28-136">Request body</span></span>
<span data-ttu-id="04f28-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="04f28-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="04f28-140">属性</span><span class="sxs-lookup"><span data-stu-id="04f28-140">Property</span></span>     | <span data-ttu-id="04f28-141">类型</span><span class="sxs-lookup"><span data-stu-id="04f28-141">Type</span></span>   |<span data-ttu-id="04f28-142">说明</span><span class="sxs-lookup"><span data-stu-id="04f28-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04f28-143">color</span><span class="sxs-lookup"><span data-stu-id="04f28-143">color</span></span>|<span data-ttu-id="04f28-144">String</span><span class="sxs-lookup"><span data-stu-id="04f28-144">String</span></span>|<span data-ttu-id="04f28-p107">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="04f28-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="04f28-147">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="04f28-147">isDefaultCalendar</span></span>|<span data-ttu-id="04f28-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f28-148">Boolean</span></span>|<span data-ttu-id="04f28-149">如果此日历是用户的默认日历，则值为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="04f28-149">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="04f28-150">name</span><span class="sxs-lookup"><span data-stu-id="04f28-150">name</span></span>|<span data-ttu-id="04f28-151">String</span><span class="sxs-lookup"><span data-stu-id="04f28-151">String</span></span>|<span data-ttu-id="04f28-152">日历名称。</span><span class="sxs-lookup"><span data-stu-id="04f28-152">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="04f28-153">响应</span><span class="sxs-lookup"><span data-stu-id="04f28-153">Response</span></span>

<span data-ttu-id="04f28-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04f28-154">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04f28-155">示例</span><span class="sxs-lookup"><span data-stu-id="04f28-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="04f28-156">请求</span><span class="sxs-lookup"><span data-stu-id="04f28-156">Request</span></span>
<span data-ttu-id="04f28-157">以下示例更新登录用户的默认日历的名称。</span><span class="sxs-lookup"><span data-stu-id="04f28-157">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="04f28-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="04f28-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="04f28-159">C#</span><span class="sxs-lookup"><span data-stu-id="04f28-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04f28-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04f28-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04f28-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04f28-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04f28-162">Java</span><span class="sxs-lookup"><span data-stu-id="04f28-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="04f28-163">响应</span><span class="sxs-lookup"><span data-stu-id="04f28-163">Response</span></span>
<span data-ttu-id="04f28-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04f28-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

