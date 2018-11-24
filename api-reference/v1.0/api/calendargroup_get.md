# <a name="get-calendargroup"></a><span data-ttu-id="69a85-101">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="69a85-101">Get calendarGroup</span></span>

<span data-ttu-id="69a85-102">检索日历组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69a85-102">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69a85-103">权限</span><span class="sxs-lookup"><span data-stu-id="69a85-103">Permissions</span></span>

<span data-ttu-id="69a85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="69a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="69a85-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="69a85-106">Permission type</span></span>                        | <span data-ttu-id="69a85-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69a85-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="69a85-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69a85-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="69a85-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69a85-109">Calendars.Read</span></span>                              |
| <span data-ttu-id="69a85-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69a85-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69a85-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69a85-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="69a85-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="69a85-112">Application</span></span>                            | <span data-ttu-id="69a85-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69a85-113">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="69a85-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69a85-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="69a85-115">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="69a85-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69a85-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69a85-116">Optional query parameters</span></span>

<span data-ttu-id="69a85-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69a85-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69a85-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="69a85-118">Request headers</span></span>

| <span data-ttu-id="69a85-119">名称</span><span class="sxs-lookup"><span data-stu-id="69a85-119">Name</span></span>          | <span data-ttu-id="69a85-120">类型</span><span class="sxs-lookup"><span data-stu-id="69a85-120">Type</span></span>   | <span data-ttu-id="69a85-121">说明</span><span class="sxs-lookup"><span data-stu-id="69a85-121">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="69a85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69a85-122">Authorization</span></span> | <span data-ttu-id="69a85-123">string</span><span class="sxs-lookup"><span data-stu-id="69a85-123">string</span></span> | <span data-ttu-id="69a85-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69a85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69a85-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69a85-126">Request body</span></span>

<span data-ttu-id="69a85-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69a85-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69a85-128">响应</span><span class="sxs-lookup"><span data-stu-id="69a85-128">Response</span></span>

<span data-ttu-id="69a85-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69a85-129">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69a85-130">示例</span><span class="sxs-lookup"><span data-stu-id="69a85-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69a85-131">请求</span><span class="sxs-lookup"><span data-stu-id="69a85-131">Request</span></span>

<span data-ttu-id="69a85-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69a85-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="69a85-133">响应</span><span class="sxs-lookup"><span data-stu-id="69a85-133">Response</span></span>

<span data-ttu-id="69a85-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69a85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
