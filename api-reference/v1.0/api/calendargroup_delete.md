# <a name="delete-calendargroup"></a><span data-ttu-id="44723-101">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="44723-101">Delete calendarGroup</span></span>

<span data-ttu-id="44723-102">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="44723-102">Delete a calendar group other than the default calendar group.</span></span>

<span data-ttu-id="44723-p101">**注意** Outlook.com 仅支持可通过 /me/calendars 快捷方式访问的默认日历组。不能删除 Outlook.com 中的任意日历组。</span><span class="sxs-lookup"><span data-stu-id="44723-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the /me/calendars shortcut. You cannot delete any calendar group in Outlook.com.</span></span>

## <a name="permissions"></a><span data-ttu-id="44723-105">权限</span><span class="sxs-lookup"><span data-stu-id="44723-105">Permissions</span></span>
<span data-ttu-id="44723-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="44723-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44723-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="44723-108">Permission type</span></span>      | <span data-ttu-id="44723-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44723-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="44723-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44723-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44723-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44723-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="44723-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44723-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44723-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44723-113">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="44723-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="44723-114">Application</span></span> | <span data-ttu-id="44723-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44723-115">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="44723-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44723-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="44723-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="44723-117">Request headers</span></span>
| <span data-ttu-id="44723-118">名称</span><span class="sxs-lookup"><span data-stu-id="44723-118">Name</span></span>       | <span data-ttu-id="44723-119">类型</span><span class="sxs-lookup"><span data-stu-id="44723-119">Type</span></span> | <span data-ttu-id="44723-120">说明</span><span class="sxs-lookup"><span data-stu-id="44723-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="44723-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44723-121">Authorization</span></span>  | <span data-ttu-id="44723-122">string</span><span class="sxs-lookup"><span data-stu-id="44723-122">string</span></span>  | <span data-ttu-id="44723-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44723-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44723-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="44723-125">Request body</span></span>
<span data-ttu-id="44723-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44723-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44723-127">响应</span><span class="sxs-lookup"><span data-stu-id="44723-127">Response</span></span>

<span data-ttu-id="44723-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="44723-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44723-130">示例</span><span class="sxs-lookup"><span data-stu-id="44723-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44723-131">请求</span><span class="sxs-lookup"><span data-stu-id="44723-131">Request</span></span>
<span data-ttu-id="44723-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44723-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="44723-133">响应</span><span class="sxs-lookup"><span data-stu-id="44723-133">Response</span></span>
<span data-ttu-id="44723-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44723-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
