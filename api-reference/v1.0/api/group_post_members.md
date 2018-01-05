# <a name="add-member"></a><span data-ttu-id="28e26-101">添加成员</span><span class="sxs-lookup"><span data-stu-id="28e26-101">Add member</span></span>
<span data-ttu-id="28e26-102">通过 **members** 导航属性，使用此 API 将成员添加到 Office 365 组、安全组或已启用邮件的安全组中。</span><span class="sxs-lookup"><span data-stu-id="28e26-102">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

<span data-ttu-id="28e26-103">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="28e26-103">You can add users or other groups.</span></span> <span data-ttu-id="28e26-104">重要说明：只能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="28e26-104">Important: You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="28e26-105">权限</span><span class="sxs-lookup"><span data-stu-id="28e26-105">Permissions</span></span>
<span data-ttu-id="28e26-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="28e26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="28e26-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="28e26-108">Permission type</span></span>      | <span data-ttu-id="28e26-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28e26-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28e26-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28e26-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28e26-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28e26-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28e26-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28e26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28e26-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="28e26-113">Not supported.</span></span>    |
|<span data-ttu-id="28e26-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="28e26-114">Application</span></span> | <span data-ttu-id="28e26-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28e26-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28e26-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28e26-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="28e26-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="28e26-117">Request headers</span></span>
| <span data-ttu-id="28e26-118">名称</span><span class="sxs-lookup"><span data-stu-id="28e26-118">Name</span></span>       | <span data-ttu-id="28e26-119">类型</span><span class="sxs-lookup"><span data-stu-id="28e26-119">Type</span></span> | <span data-ttu-id="28e26-120">说明</span><span class="sxs-lookup"><span data-stu-id="28e26-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28e26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28e26-121">Authorization</span></span>  | <span data-ttu-id="28e26-122">string</span><span class="sxs-lookup"><span data-stu-id="28e26-122">string</span></span>  | <span data-ttu-id="28e26-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28e26-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28e26-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="28e26-125">Request body</span></span>
<span data-ttu-id="28e26-126">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28e26-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="28e26-127">响应</span><span class="sxs-lookup"><span data-stu-id="28e26-127">Response</span></span>
<span data-ttu-id="28e26-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="28e26-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e26-130">示例</span><span class="sxs-lookup"><span data-stu-id="28e26-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="28e26-131">请求</span><span class="sxs-lookup"><span data-stu-id="28e26-131">Request</span></span>
<span data-ttu-id="28e26-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28e26-132">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="28e26-133">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 `id` 的JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28e26-133">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="28e26-134">响应</span><span class="sxs-lookup"><span data-stu-id="28e26-134">Response</span></span>
<span data-ttu-id="28e26-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28e26-135">Here is an example of the response.</span></span>
><span data-ttu-id="28e26-136">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="28e26-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="28e26-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="28e26-137">All the properties will be returned from an actual call.</span></span>
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