# <a name="delete-domain"></a><span data-ttu-id="9ece2-101">删除域</span><span class="sxs-lookup"><span data-stu-id="9ece2-101">Delete domain</span></span>

<span data-ttu-id="9ece2-102">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="9ece2-102">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="9ece2-103">**重要说明：**</span><span class="sxs-lookup"><span data-stu-id="9ece2-103">**Important:**</span></span>
> - <span data-ttu-id="9ece2-104">已删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="9ece2-104">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="9ece2-p101">如果存在任何仍旧依赖域的资源或对象，尝试删除会失败。可以通过使用此 [列出 domainNameReferences](domain_list_domainnamereferences.md) API 查找所有从属的资源。</span><span class="sxs-lookup"><span data-stu-id="9ece2-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain_list_domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ece2-107">权限</span><span class="sxs-lookup"><span data-stu-id="9ece2-107">Permissions</span></span>

<span data-ttu-id="9ece2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9ece2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9ece2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ece2-110">Permission type</span></span>      | <span data-ttu-id="9ece2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ece2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ece2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ece2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ece2-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ece2-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ece2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ece2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ece2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ece2-115">Not supported.</span></span>    |
|<span data-ttu-id="9ece2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ece2-116">Application</span></span> | <span data-ttu-id="9ece2-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ece2-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ece2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ece2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="9ece2-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="9ece2-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ece2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ece2-120">Request headers</span></span>

| <span data-ttu-id="9ece2-121">名称</span><span class="sxs-lookup"><span data-stu-id="9ece2-121">Name</span></span>       | <span data-ttu-id="9ece2-122">说明</span><span class="sxs-lookup"><span data-stu-id="9ece2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ece2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ece2-123">Authorization</span></span>  | <span data-ttu-id="9ece2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ece2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ece2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ece2-126">Content-Type</span></span>  | <span data-ttu-id="9ece2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ece2-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ece2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ece2-128">Request body</span></span>

<span data-ttu-id="9ece2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ece2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ece2-130">响应</span><span class="sxs-lookup"><span data-stu-id="9ece2-130">Response</span></span>

<span data-ttu-id="9ece2-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="9ece2-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ece2-133">示例</span><span class="sxs-lookup"><span data-stu-id="9ece2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ece2-134">请求</span><span class="sxs-lookup"><span data-stu-id="9ece2-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="9ece2-135">响应</span><span class="sxs-lookup"><span data-stu-id="9ece2-135">Response</span></span>

<span data-ttu-id="9ece2-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ece2-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->