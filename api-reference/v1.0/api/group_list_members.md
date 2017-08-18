# <a name="list-members"></a><span data-ttu-id="a6483-101">列出成员</span><span class="sxs-lookup"><span data-stu-id="a6483-101">List members</span></span>

<span data-ttu-id="a6483-p101">获取组的直接成员列表。组可将用户、联系人和其他组作为成员。此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="a6483-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6483-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6483-105">Prerequisites</span></span>
<span data-ttu-id="a6483-106">要执行此 API，需要以下**范围**之一：*Directory.Read.All*、*Directory.AccessAsUser.All*、*User.ReadBasic.All* 或 *User.Read.All*</span><span class="sxs-lookup"><span data-stu-id="a6483-106">One of the following **scopes** is required to execute this API: *Directory.Read.All*, *Directory.AccessAsUser.All*, *User.ReadBasic.All*, or *User.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="a6483-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6483-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6483-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6483-108">Optional query parameters</span></span>
<span data-ttu-id="a6483-109">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a6483-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a6483-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6483-110">Request headers</span></span>
| <span data-ttu-id="a6483-111">名称</span><span class="sxs-lookup"><span data-stu-id="a6483-111">Name</span></span>       | <span data-ttu-id="a6483-112">类型</span><span class="sxs-lookup"><span data-stu-id="a6483-112">Type</span></span> | <span data-ttu-id="a6483-113">说明</span><span class="sxs-lookup"><span data-stu-id="a6483-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a6483-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6483-114">Authorization</span></span>  | <span data-ttu-id="a6483-115">string</span><span class="sxs-lookup"><span data-stu-id="a6483-115">string</span></span>  | <span data-ttu-id="a6483-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6483-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6483-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6483-118">Request body</span></span>
<span data-ttu-id="a6483-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6483-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6483-120">响应</span><span class="sxs-lookup"><span data-stu-id="a6483-120">Response</span></span>

<span data-ttu-id="a6483-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6483-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6483-122">示例</span><span class="sxs-lookup"><span data-stu-id="a6483-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6483-123">请求</span><span class="sxs-lookup"><span data-stu-id="a6483-123">Request</span></span>
<span data-ttu-id="a6483-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6483-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="a6483-125">响应</span><span class="sxs-lookup"><span data-stu-id="a6483-125">Response</span></span>
<span data-ttu-id="a6483-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6483-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->