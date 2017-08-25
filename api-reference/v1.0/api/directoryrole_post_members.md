# <a name="add-directory-role-member"></a><span data-ttu-id="76130-101">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="76130-101">Add directory role member</span></span>

<span data-ttu-id="76130-102">使用此 API 创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="76130-102">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="76130-103">权限</span><span class="sxs-lookup"><span data-stu-id="76130-103">Permissions</span></span>
<span data-ttu-id="76130-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="76130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76130-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="76130-106">Permission type</span></span>      | <span data-ttu-id="76130-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76130-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="76130-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76130-108">Delegated (work or school account)</span></span> | <span data-ttu-id="76130-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76130-109">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="76130-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76130-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76130-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="76130-111">Not supported.</span></span>    | 
|<span data-ttu-id="76130-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="76130-112">Application</span></span> | <span data-ttu-id="76130-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="76130-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="76130-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76130-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="76130-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="76130-115">Request headers</span></span>
| <span data-ttu-id="76130-116">名称</span><span class="sxs-lookup"><span data-stu-id="76130-116">Name</span></span>       | <span data-ttu-id="76130-117">类型</span><span class="sxs-lookup"><span data-stu-id="76130-117">Type</span></span> | <span data-ttu-id="76130-118">说明</span><span class="sxs-lookup"><span data-stu-id="76130-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76130-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="76130-119">Authorization</span></span>  | <span data-ttu-id="76130-120">string</span><span class="sxs-lookup"><span data-stu-id="76130-120">string</span></span>  | <span data-ttu-id="76130-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76130-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76130-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76130-123">Content-Type</span></span>  | <span data-ttu-id="76130-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76130-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76130-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="76130-125">Request body</span></span>
<span data-ttu-id="76130-126">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76130-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="76130-127">响应</span><span class="sxs-lookup"><span data-stu-id="76130-127">Response</span></span>

<span data-ttu-id="76130-128">如果成功，此方法返回 `204, No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="76130-128">If successful, this method returns `204, No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76130-129">示例</span><span class="sxs-lookup"><span data-stu-id="76130-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76130-130">请求</span><span class="sxs-lookup"><span data-stu-id="76130-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="76130-131">响应</span><span class="sxs-lookup"><span data-stu-id="76130-131">Response</span></span>
<span data-ttu-id="76130-132">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="76130-132">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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