# <a name="update-domain"></a><span data-ttu-id="28eeb-101">更新域</span><span class="sxs-lookup"><span data-stu-id="28eeb-101">Update domain</span></span>

<span data-ttu-id="28eeb-102">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28eeb-102">Update the properties of domain object.</span></span>

> <span data-ttu-id="28eeb-103">**重要说明：**只有已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="28eeb-103">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="28eeb-104">权限</span><span class="sxs-lookup"><span data-stu-id="28eeb-104">Permissions</span></span>

<span data-ttu-id="28eeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="28eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="28eeb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="28eeb-107">Permission type</span></span>      | <span data-ttu-id="28eeb-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28eeb-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28eeb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28eeb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="28eeb-110">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28eeb-110">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28eeb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28eeb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28eeb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="28eeb-112">Not supported.</span></span>    |
|<span data-ttu-id="28eeb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="28eeb-113">Application</span></span> | <span data-ttu-id="28eeb-114">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28eeb-114">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28eeb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28eeb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="28eeb-116">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="28eeb-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28eeb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="28eeb-117">Request headers</span></span>

| <span data-ttu-id="28eeb-118">名称</span><span class="sxs-lookup"><span data-stu-id="28eeb-118">Name</span></span>       | <span data-ttu-id="28eeb-119">说明</span><span class="sxs-lookup"><span data-stu-id="28eeb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="28eeb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="28eeb-120">Authorization</span></span>  | <span data-ttu-id="28eeb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28eeb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28eeb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28eeb-123">Content-Type</span></span>  | <span data-ttu-id="28eeb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28eeb-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="28eeb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="28eeb-125">Request body</span></span>

<span data-ttu-id="28eeb-p103">在请求正文中，提供要更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，仅包含已更改的值。</span><span class="sxs-lookup"><span data-stu-id="28eeb-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="28eeb-129">响应</span><span class="sxs-lookup"><span data-stu-id="28eeb-129">Response</span></span>

<span data-ttu-id="28eeb-130">如果成功，此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="28eeb-130">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="28eeb-131">示例</span><span class="sxs-lookup"><span data-stu-id="28eeb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28eeb-132">请求</span><span class="sxs-lookup"><span data-stu-id="28eeb-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="28eeb-133">响应</span><span class="sxs-lookup"><span data-stu-id="28eeb-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->