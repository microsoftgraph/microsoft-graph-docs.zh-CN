# <a name="filter-clear"></a><span data-ttu-id="cbd6c-101">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="cbd6c-101">Filter: clear</span></span>

<span data-ttu-id="cbd6c-102">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-102">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbd6c-103">权限</span><span class="sxs-lookup"><span data-stu-id="cbd6c-103">Permissions</span></span>
<span data-ttu-id="cbd6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cbd6c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbd6c-106">Permission type</span></span>      | <span data-ttu-id="cbd6c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cbd6c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbd6c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd6c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cbd6c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbd6c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbd6c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd6c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbd6c-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-111">Not supported.</span></span>    |
|<span data-ttu-id="cbd6c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbd6c-112">Application</span></span> | <span data-ttu-id="cbd6c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbd6c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbd6c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="cbd6c-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbd6c-115">Request headers</span></span>
| <span data-ttu-id="cbd6c-116">名称</span><span class="sxs-lookup"><span data-stu-id="cbd6c-116">Name</span></span>       | <span data-ttu-id="cbd6c-117">说明</span><span class="sxs-lookup"><span data-stu-id="cbd6c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cbd6c-118">授权</span><span class="sxs-lookup"><span data-stu-id="cbd6c-118">Authorization</span></span>  | <span data-ttu-id="cbd6c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbd6c-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbd6c-121">Request body</span></span>
<span data-ttu-id="cbd6c-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd6c-123">响应</span><span class="sxs-lookup"><span data-stu-id="cbd6c-123">Response</span></span>

<span data-ttu-id="cbd6c-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbd6c-126">示例</span><span class="sxs-lookup"><span data-stu-id="cbd6c-126">Example</span></span>
<span data-ttu-id="cbd6c-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cbd6c-128">请求</span><span class="sxs-lookup"><span data-stu-id="cbd6c-128">Request</span></span>
<span data-ttu-id="cbd6c-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="cbd6c-130">响应</span><span class="sxs-lookup"><span data-stu-id="cbd6c-130">Response</span></span>
<span data-ttu-id="cbd6c-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cbd6c-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->