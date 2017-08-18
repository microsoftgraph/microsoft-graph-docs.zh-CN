# <a name="range-clear"></a><span data-ttu-id="d6291-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="d6291-101">Range: clear</span></span>

<span data-ttu-id="d6291-102">清除区域值、格式、填充、边框等。</span><span class="sxs-lookup"><span data-stu-id="d6291-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6291-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6291-103">Prerequisites</span></span>
<span data-ttu-id="d6291-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="d6291-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="d6291-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6291-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="d6291-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6291-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="d6291-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6291-107">Request headers</span></span>
| <span data-ttu-id="d6291-108">名称</span><span class="sxs-lookup"><span data-stu-id="d6291-108">Name</span></span>       | <span data-ttu-id="d6291-109">说明</span><span class="sxs-lookup"><span data-stu-id="d6291-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d6291-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6291-110">Authorization</span></span>  | <span data-ttu-id="d6291-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6291-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d6291-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6291-113">Request body</span></span>
<span data-ttu-id="d6291-114">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d6291-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d6291-115">参数</span><span class="sxs-lookup"><span data-stu-id="d6291-115">Parameter</span></span>    | <span data-ttu-id="d6291-116">类型</span><span class="sxs-lookup"><span data-stu-id="d6291-116">Type</span></span>   |<span data-ttu-id="d6291-117">说明</span><span class="sxs-lookup"><span data-stu-id="d6291-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6291-118">applyTo</span><span class="sxs-lookup"><span data-stu-id="d6291-118">applyTo</span></span>|<span data-ttu-id="d6291-119">string</span><span class="sxs-lookup"><span data-stu-id="d6291-119">string</span></span>|<span data-ttu-id="d6291-p102">可选。确定清除操作的类型。可能的值是：`All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="d6291-p102">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="d6291-123">响应</span><span class="sxs-lookup"><span data-stu-id="d6291-123">Response</span></span>

<span data-ttu-id="d6291-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d6291-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6291-126">示例</span><span class="sxs-lookup"><span data-stu-id="d6291-126">Example</span></span>
<span data-ttu-id="d6291-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d6291-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d6291-128">请求</span><span class="sxs-lookup"><span data-stu-id="d6291-128">Request</span></span>
<span data-ttu-id="d6291-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6291-129">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d6291-130">响应</span><span class="sxs-lookup"><span data-stu-id="d6291-130">Response</span></span>
<span data-ttu-id="d6291-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d6291-131">Here is an example of the response.</span></span> 
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