# <a name="remove-owner"></a><span data-ttu-id="a04e4-101">删除所有者</span><span class="sxs-lookup"><span data-stu-id="a04e4-101">Remove owner</span></span>
<span data-ttu-id="a04e4-102">使用此 API 可以通过 owners 导航属性删除 Office 365 组、安全组或已启用邮件的安全组中的所有者。</span><span class="sxs-lookup"><span data-stu-id="a04e4-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a04e4-103">权限</span><span class="sxs-lookup"><span data-stu-id="a04e4-103">Permissions</span></span>
<span data-ttu-id="a04e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a04e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a04e4-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="a04e4-106">Permission type</span></span>      | <span data-ttu-id="a04e4-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a04e4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a04e4-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a04e4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a04e4-109">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a04e4-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a04e4-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a04e4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a04e4-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a04e4-111">Not supported.</span></span>    |
|<span data-ttu-id="a04e4-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="a04e4-112">Application</span></span> | <span data-ttu-id="a04e4-113">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a04e4-113">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a04e4-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a04e4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a04e4-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="a04e4-115">Request headers</span></span>
| <span data-ttu-id="a04e4-116">名称</span><span class="sxs-lookup"><span data-stu-id="a04e4-116">Name</span></span>       | <span data-ttu-id="a04e4-117">类型</span><span class="sxs-lookup"><span data-stu-id="a04e4-117">Type</span></span> | <span data-ttu-id="a04e4-118">说明</span><span class="sxs-lookup"><span data-stu-id="a04e4-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a04e4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a04e4-119">Authorization</span></span>  | <span data-ttu-id="a04e4-120">string</span><span class="sxs-lookup"><span data-stu-id="a04e4-120">string</span></span>  | <span data-ttu-id="a04e4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a04e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a04e4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a04e4-123">Request body</span></span>
<span data-ttu-id="a04e4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a04e4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a04e4-125">响应</span><span class="sxs-lookup"><span data-stu-id="a04e4-125">Response</span></span>
<span data-ttu-id="a04e4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a04e4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a04e4-128">示例</span><span class="sxs-lookup"><span data-stu-id="a04e4-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a04e4-129">请求</span><span class="sxs-lookup"><span data-stu-id="a04e4-129">Request</span></span>
<span data-ttu-id="a04e4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a04e4-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="a04e4-131">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="a04e4-131">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="a04e4-132">响应</span><span class="sxs-lookup"><span data-stu-id="a04e4-132">Response</span></span>
<span data-ttu-id="a04e4-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a04e4-133">Here is an example of the response.</span></span>
><span data-ttu-id="a04e4-134">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a04e4-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a04e4-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a04e4-135">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
