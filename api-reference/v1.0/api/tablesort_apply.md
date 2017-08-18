# <a name="tablesort-apply"></a><span data-ttu-id="edaf0-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="edaf0-101">TableSort: apply</span></span>

<span data-ttu-id="edaf0-102">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="edaf0-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edaf0-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="edaf0-103">Prerequisites</span></span>
<span data-ttu-id="edaf0-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="edaf0-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="edaf0-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edaf0-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="edaf0-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edaf0-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="edaf0-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="edaf0-107">Request headers</span></span>
| <span data-ttu-id="edaf0-108">名称</span><span class="sxs-lookup"><span data-stu-id="edaf0-108">Name</span></span>       | <span data-ttu-id="edaf0-109">说明</span><span class="sxs-lookup"><span data-stu-id="edaf0-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="edaf0-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="edaf0-110">Authorization</span></span>  | <span data-ttu-id="edaf0-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edaf0-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="edaf0-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="edaf0-113">Request body</span></span>
<span data-ttu-id="edaf0-114">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="edaf0-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="edaf0-115">参数</span><span class="sxs-lookup"><span data-stu-id="edaf0-115">Parameter</span></span>    | <span data-ttu-id="edaf0-116">类型</span><span class="sxs-lookup"><span data-stu-id="edaf0-116">Type</span></span>   |<span data-ttu-id="edaf0-117">说明</span><span class="sxs-lookup"><span data-stu-id="edaf0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edaf0-118">fields</span><span class="sxs-lookup"><span data-stu-id="edaf0-118">fields</span></span>|<span data-ttu-id="edaf0-119">SortField</span><span class="sxs-lookup"><span data-stu-id="edaf0-119">SortField</span></span>|<span data-ttu-id="edaf0-120">作为排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="edaf0-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="edaf0-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="edaf0-121">matchCase</span></span>|<span data-ttu-id="edaf0-122">boolean</span><span class="sxs-lookup"><span data-stu-id="edaf0-122">boolean</span></span>|<span data-ttu-id="edaf0-p102">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="edaf0-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="edaf0-125">method</span><span class="sxs-lookup"><span data-stu-id="edaf0-125">method</span></span>|<span data-ttu-id="edaf0-126">string</span><span class="sxs-lookup"><span data-stu-id="edaf0-126">string</span></span>|<span data-ttu-id="edaf0-p103">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="edaf0-p103">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="edaf0-130">响应</span><span class="sxs-lookup"><span data-stu-id="edaf0-130">Response</span></span>

<span data-ttu-id="edaf0-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="edaf0-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edaf0-133">示例</span><span class="sxs-lookup"><span data-stu-id="edaf0-133">Example</span></span>
<span data-ttu-id="edaf0-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="edaf0-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="edaf0-135">请求</span><span class="sxs-lookup"><span data-stu-id="edaf0-135">Request</span></span>
<span data-ttu-id="edaf0-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edaf0-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="edaf0-137">响应</span><span class="sxs-lookup"><span data-stu-id="edaf0-137">Response</span></span>
<span data-ttu-id="edaf0-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="edaf0-138">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->