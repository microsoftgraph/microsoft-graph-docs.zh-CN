# <a name="range-clear"></a><span data-ttu-id="966e4-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="966e4-101">Range: clear</span></span>

<span data-ttu-id="966e4-102">清除范围值、格式、填充、边框等。</span><span class="sxs-lookup"><span data-stu-id="966e4-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="966e4-103">权限</span><span class="sxs-lookup"><span data-stu-id="966e4-103">Permissions</span></span>
<span data-ttu-id="966e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="966e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="966e4-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="966e4-106">Permission type</span></span>      | <span data-ttu-id="966e4-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="966e4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="966e4-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="966e4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="966e4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="966e4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="966e4-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="966e4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="966e4-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="966e4-111">Not supported.</span></span>    |
|<span data-ttu-id="966e4-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="966e4-112">Application</span></span> | <span data-ttu-id="966e4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="966e4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="966e4-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="966e4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="966e4-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="966e4-115">Request headers</span></span>
| <span data-ttu-id="966e4-116">名称</span><span class="sxs-lookup"><span data-stu-id="966e4-116">Name</span></span>       | <span data-ttu-id="966e4-117">说明</span><span class="sxs-lookup"><span data-stu-id="966e4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="966e4-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="966e4-118">Authorization</span></span>  | <span data-ttu-id="966e4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="966e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="966e4-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="966e4-121">Request body</span></span>
<span data-ttu-id="966e4-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="966e4-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="966e4-123">参数</span><span class="sxs-lookup"><span data-stu-id="966e4-123">Parameter</span></span>    | <span data-ttu-id="966e4-124">类型</span><span class="sxs-lookup"><span data-stu-id="966e4-124">Type</span></span>   |<span data-ttu-id="966e4-125">说明</span><span class="sxs-lookup"><span data-stu-id="966e4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="966e4-126">applyTo</span><span class="sxs-lookup"><span data-stu-id="966e4-126">applyTo</span></span>|<span data-ttu-id="966e4-127">string</span><span class="sxs-lookup"><span data-stu-id="966e4-127">string</span></span>|<span data-ttu-id="966e4-p103">可选。确定清除操作的类型。可能的值是：`All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="966e4-p103">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="966e4-131">响应</span><span class="sxs-lookup"><span data-stu-id="966e4-131">Response</span></span>

<span data-ttu-id="966e4-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="966e4-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="966e4-134">示例</span><span class="sxs-lookup"><span data-stu-id="966e4-134">Example</span></span>
<span data-ttu-id="966e4-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="966e4-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="966e4-136">请求</span><span class="sxs-lookup"><span data-stu-id="966e4-136">Request</span></span>
<span data-ttu-id="966e4-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="966e4-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="966e4-138">响应</span><span class="sxs-lookup"><span data-stu-id="966e4-138">Response</span></span>
<span data-ttu-id="966e4-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="966e4-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->