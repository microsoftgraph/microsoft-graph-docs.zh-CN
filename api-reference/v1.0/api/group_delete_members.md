# <a name="remove-member"></a><span data-ttu-id="80fd8-101">删除成员</span><span class="sxs-lookup"><span data-stu-id="80fd8-101">Remove member</span></span>
<span data-ttu-id="80fd8-p101">使用此 API 可以通过 **members** 导航属性删除 Office 365 组、安全组或已启用邮件的安全组中的成员。你可以删除用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="80fd8-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="80fd8-104">权限</span><span class="sxs-lookup"><span data-stu-id="80fd8-104">Permissions</span></span>
<span data-ttu-id="80fd8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="80fd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80fd8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="80fd8-107">Permission type</span></span>      | <span data-ttu-id="80fd8-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80fd8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80fd8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80fd8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="80fd8-110">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80fd8-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80fd8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80fd8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80fd8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="80fd8-112">Not supported.</span></span>    |
|<span data-ttu-id="80fd8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="80fd8-113">Application</span></span> | <span data-ttu-id="80fd8-114">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80fd8-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="80fd8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80fd8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="80fd8-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="80fd8-116">Request headers</span></span>
| <span data-ttu-id="80fd8-117">名称</span><span class="sxs-lookup"><span data-stu-id="80fd8-117">Name</span></span>       | <span data-ttu-id="80fd8-118">类型</span><span class="sxs-lookup"><span data-stu-id="80fd8-118">Type</span></span> | <span data-ttu-id="80fd8-119">说明</span><span class="sxs-lookup"><span data-stu-id="80fd8-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80fd8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="80fd8-120">Authorization</span></span>  | <span data-ttu-id="80fd8-121">string</span><span class="sxs-lookup"><span data-stu-id="80fd8-121">string</span></span>  | <span data-ttu-id="80fd8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80fd8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80fd8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="80fd8-124">Request body</span></span>
<span data-ttu-id="80fd8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80fd8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80fd8-126">响应</span><span class="sxs-lookup"><span data-stu-id="80fd8-126">Response</span></span>
<span data-ttu-id="80fd8-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="80fd8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80fd8-129">示例</span><span class="sxs-lookup"><span data-stu-id="80fd8-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="80fd8-130">请求</span><span class="sxs-lookup"><span data-stu-id="80fd8-130">Request</span></span>
<span data-ttu-id="80fd8-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80fd8-131">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="80fd8-132">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="80fd8-132">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="80fd8-133">响应</span><span class="sxs-lookup"><span data-stu-id="80fd8-133">Response</span></span>
<span data-ttu-id="80fd8-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80fd8-134">Here is an example of the response.</span></span>
><span data-ttu-id="80fd8-135">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80fd8-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80fd8-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="80fd8-136">All the properties will be returned from an actual call.</span></span>
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