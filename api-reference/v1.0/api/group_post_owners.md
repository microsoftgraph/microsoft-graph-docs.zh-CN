# <a name="add-group-owner"></a><span data-ttu-id="c3272-101">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="c3272-101">Add group owner</span></span>
<span data-ttu-id="c3272-p101">将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="c3272-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3272-104">权限</span><span class="sxs-lookup"><span data-stu-id="c3272-104">Permissions</span></span>
<span data-ttu-id="c3272-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c3272-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c3272-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3272-107">Permission type</span></span>      | <span data-ttu-id="c3272-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3272-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3272-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3272-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c3272-110">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3272-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c3272-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3272-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3272-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3272-112">Not supported.</span></span>    |
|<span data-ttu-id="c3272-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3272-113">Application</span></span> | <span data-ttu-id="c3272-114">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3272-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3272-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3272-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c3272-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3272-116">Request headers</span></span>
| <span data-ttu-id="c3272-117">名称</span><span class="sxs-lookup"><span data-stu-id="c3272-117">Name</span></span>       | <span data-ttu-id="c3272-118">类型</span><span class="sxs-lookup"><span data-stu-id="c3272-118">Type</span></span> | <span data-ttu-id="c3272-119">说明</span><span class="sxs-lookup"><span data-stu-id="c3272-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3272-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3272-120">Authorization</span></span>  | <span data-ttu-id="c3272-121">string</span><span class="sxs-lookup"><span data-stu-id="c3272-121">string</span></span>  | <span data-ttu-id="c3272-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3272-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3272-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3272-124">Request body</span></span>
<span data-ttu-id="c3272-125">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3272-125">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c3272-126">响应</span><span class="sxs-lookup"><span data-stu-id="c3272-126">Response</span></span>
<span data-ttu-id="c3272-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c3272-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3272-129">示例</span><span class="sxs-lookup"><span data-stu-id="c3272-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c3272-130">请求</span><span class="sxs-lookup"><span data-stu-id="c3272-130">Request</span></span>
<span data-ttu-id="c3272-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c3272-131">The following is an example of the request body.</span></span>
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
<span data-ttu-id="c3272-132">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3272-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="c3272-133">响应</span><span class="sxs-lookup"><span data-stu-id="c3272-133">Response</span></span>
<span data-ttu-id="c3272-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c3272-134">Here is an example of the response.</span></span>
><span data-ttu-id="c3272-135">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c3272-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3272-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c3272-136">All the properties will be returned from an actual call.</span></span>
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
