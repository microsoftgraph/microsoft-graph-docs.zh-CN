# <a name="assign-a-manager"></a><span data-ttu-id="d92c0-101">指定经理</span><span class="sxs-lookup"><span data-stu-id="d92c0-101">Assign a manager</span></span>

<span data-ttu-id="d92c0-102">使用此 API 指定用户的经理。</span><span class="sxs-lookup"><span data-stu-id="d92c0-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="d92c0-103">注意：不能指定直接下属，请改用此 API。</span><span class="sxs-lookup"><span data-stu-id="d92c0-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d92c0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d92c0-104">Prerequisites</span></span>
<span data-ttu-id="d92c0-105">要执行此 API，需要以下**范围**之一：*Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="d92c0-105">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="d92c0-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d92c0-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d92c0-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="d92c0-107">Request headers</span></span>
| <span data-ttu-id="d92c0-108">名称</span><span class="sxs-lookup"><span data-stu-id="d92c0-108">Name</span></span>       | <span data-ttu-id="d92c0-109">类型</span><span class="sxs-lookup"><span data-stu-id="d92c0-109">Type</span></span> | <span data-ttu-id="d92c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d92c0-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d92c0-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="d92c0-111">Authorization</span></span>  | <span data-ttu-id="d92c0-112">string</span><span class="sxs-lookup"><span data-stu-id="d92c0-112">string</span></span>  | <span data-ttu-id="d92c0-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d92c0-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d92c0-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="d92c0-115">Request body</span></span>
<span data-ttu-id="d92c0-116">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d92c0-116">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d92c0-117">响应</span><span class="sxs-lookup"><span data-stu-id="d92c0-117">Response</span></span>

<span data-ttu-id="d92c0-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d92c0-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d92c0-120">示例</span><span class="sxs-lookup"><span data-stu-id="d92c0-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d92c0-121">请求</span><span class="sxs-lookup"><span data-stu-id="d92c0-121">Request</span></span>
<span data-ttu-id="d92c0-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d92c0-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="d92c0-123">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d92c0-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="d92c0-124">响应</span><span class="sxs-lookup"><span data-stu-id="d92c0-124">Response</span></span>
<span data-ttu-id="d92c0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d92c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
