# <a name="add-group-owner"></a><span data-ttu-id="6d1bd-101">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="6d1bd-101">Add group owner</span></span>
<span data-ttu-id="6d1bd-p101">将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d1bd-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d1bd-104">Prerequisites</span></span>
<span data-ttu-id="6d1bd-105">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All* 或 *Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="6d1bd-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6d1bd-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d1bd-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6d1bd-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d1bd-107">Request headers</span></span>
| <span data-ttu-id="6d1bd-108">名称</span><span class="sxs-lookup"><span data-stu-id="6d1bd-108">Name</span></span>       | <span data-ttu-id="6d1bd-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d1bd-109">Type</span></span> | <span data-ttu-id="6d1bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d1bd-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d1bd-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d1bd-111">Authorization</span></span>  | <span data-ttu-id="6d1bd-112">string</span><span class="sxs-lookup"><span data-stu-id="6d1bd-112">string</span></span>  | <span data-ttu-id="6d1bd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d1bd-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d1bd-115">Request body</span></span>
<span data-ttu-id="6d1bd-116">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-116">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="6d1bd-117">响应</span><span class="sxs-lookup"><span data-stu-id="6d1bd-117">Response</span></span>

<span data-ttu-id="6d1bd-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d1bd-120">示例</span><span class="sxs-lookup"><span data-stu-id="6d1bd-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d1bd-121">请求</span><span class="sxs-lookup"><span data-stu-id="6d1bd-121">Request</span></span>
<span data-ttu-id="6d1bd-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="6d1bd-123">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="6d1bd-124">响应</span><span class="sxs-lookup"><span data-stu-id="6d1bd-124">Response</span></span>
<span data-ttu-id="6d1bd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d1bd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
