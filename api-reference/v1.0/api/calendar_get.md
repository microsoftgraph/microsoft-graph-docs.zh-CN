# <a name="get-calendar"></a><span data-ttu-id="ce6fc-101">Get calendar</span><span class="sxs-lookup"><span data-stu-id="ce6fc-101">Get calendar</span></span>

<span data-ttu-id="ce6fc-102">获取 [calendar](../resources/calendar.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="ce6fc-103">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>


### <a name="get-another-users-calendar"></a><span data-ttu-id="ce6fc-104">获取其他用户的日历</span><span class="sxs-lookup"><span data-stu-id="ce6fc-104">Get another user's calendar</span></span>

<span data-ttu-id="ce6fc-105">如果你具有应用程序权限，或者具有某个用户的适当的委派[权限](#permissions)，则可以获取其他用户的日历。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get a calendar of another user's.</span></span> <span data-ttu-id="ce6fc-106">本部分重点介绍涉及委派权限的应用场景。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="ce6fc-107">例如，你的应用已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="ce6fc-108">假设另一位用户 Garth 与 John 共享了一个日历。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-108">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="ce6fc-109">可以通过在下面所示的查询示例中指定 Garth 的用户 ID（或者用户主体名称）来获取该共享日历。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-109">You can get that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="ce6fc-110">此功能适用于对单个用户执行的所有支持的 GET 日历操作，如下面的 [HTTP 请求](#http-request)部分所示。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-110">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="ce6fc-111">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="ce6fc-112">如果 Garth 未与 John 共享他的日历，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-112">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="ce6fc-113">在这种情况下，指定用户 ID 或用户主体名称只适用于获取已登录用户的日历，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="ce6fc-113">In such cases, specifying a user ID or user principal name only works for getting a calendar of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar
```

<span data-ttu-id="ce6fc-114">此功能仅适用于以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="ce6fc-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="ce6fc-115">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="ce6fc-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="ce6fc-116">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="ce6fc-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="ce6fc-117">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="ce6fc-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="ce6fc-118">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="ce6fc-119">权限</span><span class="sxs-lookup"><span data-stu-id="ce6fc-119">Permissions</span></span>
<span data-ttu-id="ce6fc-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce6fc-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce6fc-122">Permission type</span></span>      | <span data-ttu-id="ce6fc-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce6fc-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce6fc-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce6fc-124">Delegated (work or school account)</span></span> | <span data-ttu-id="ce6fc-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ce6fc-125">Calendars.Read</span></span>    |
|<span data-ttu-id="ce6fc-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce6fc-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce6fc-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ce6fc-127">Calendars.Read</span></span>    |
|<span data-ttu-id="ce6fc-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce6fc-128">Application</span></span> | <span data-ttu-id="ce6fc-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ce6fc-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce6fc-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce6fc-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ce6fc-131">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-131">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="ce6fc-132">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-132">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="ce6fc-133">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-133">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce6fc-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce6fc-134">Optional query parameters</span></span>
<span data-ttu-id="ce6fc-135">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-135">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ce6fc-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce6fc-136">Request headers</span></span>
| <span data-ttu-id="ce6fc-137">名称</span><span class="sxs-lookup"><span data-stu-id="ce6fc-137">Name</span></span>       | <span data-ttu-id="ce6fc-138">类型</span><span class="sxs-lookup"><span data-stu-id="ce6fc-138">Type</span></span> | <span data-ttu-id="ce6fc-139">说明</span><span class="sxs-lookup"><span data-stu-id="ce6fc-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce6fc-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce6fc-140">Authorization</span></span>  | <span data-ttu-id="ce6fc-141">string</span><span class="sxs-lookup"><span data-stu-id="ce6fc-141">string</span></span>  | <span data-ttu-id="ce6fc-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce6fc-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce6fc-144">Request body</span></span>
<span data-ttu-id="ce6fc-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce6fc-146">响应</span><span class="sxs-lookup"><span data-stu-id="ce6fc-146">Response</span></span>

<span data-ttu-id="ce6fc-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-147">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce6fc-148">示例</span><span class="sxs-lookup"><span data-stu-id="ce6fc-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce6fc-149">请求</span><span class="sxs-lookup"><span data-stu-id="ce6fc-149">Request</span></span>
<span data-ttu-id="ce6fc-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="ce6fc-151">响应</span><span class="sxs-lookup"><span data-stu-id="ce6fc-151">Response</span></span>
<span data-ttu-id="ce6fc-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce6fc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
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
  "tocPath": ""
}-->
