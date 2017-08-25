# <a name="delete-calendar"></a><span data-ttu-id="de8ea-101">删除日历</span><span class="sxs-lookup"><span data-stu-id="de8ea-101">Delete calendar</span></span>

<span data-ttu-id="de8ea-102">删除默认日历以外的日历。</span><span class="sxs-lookup"><span data-stu-id="de8ea-102">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="de8ea-103">权限</span><span class="sxs-lookup"><span data-stu-id="de8ea-103">Permissions</span></span>
<span data-ttu-id="de8ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="de8ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="de8ea-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="de8ea-106">Permission type</span></span>      | <span data-ttu-id="de8ea-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de8ea-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="de8ea-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de8ea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="de8ea-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de8ea-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="de8ea-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de8ea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de8ea-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de8ea-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="de8ea-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="de8ea-112">Application</span></span> | <span data-ttu-id="de8ea-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de8ea-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="de8ea-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de8ea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="de8ea-115">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="de8ea-115">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="de8ea-116">指定 [calendarGroup](../resources/calendargroup.md) 中的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="de8ea-116">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="de8ea-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="de8ea-117">Request headers</span></span>
| <span data-ttu-id="de8ea-118">名称</span><span class="sxs-lookup"><span data-stu-id="de8ea-118">Name</span></span>           |  <span data-ttu-id="de8ea-119">类型</span><span class="sxs-lookup"><span data-stu-id="de8ea-119">Type</span></span>    | <span data-ttu-id="de8ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="de8ea-120">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="de8ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de8ea-121">Authorization</span></span>  |  <span data-ttu-id="de8ea-122">string</span><span class="sxs-lookup"><span data-stu-id="de8ea-122">string</span></span>  | <span data-ttu-id="de8ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de8ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de8ea-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="de8ea-125">Request body</span></span>
<span data-ttu-id="de8ea-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de8ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de8ea-127">响应</span><span class="sxs-lookup"><span data-stu-id="de8ea-127">Response</span></span>

<span data-ttu-id="de8ea-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="de8ea-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de8ea-130">示例</span><span class="sxs-lookup"><span data-stu-id="de8ea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de8ea-131">请求</span><span class="sxs-lookup"><span data-stu-id="de8ea-131">Request</span></span>
<span data-ttu-id="de8ea-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de8ea-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="de8ea-133">响应</span><span class="sxs-lookup"><span data-stu-id="de8ea-133">Response</span></span>
<span data-ttu-id="de8ea-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="de8ea-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
