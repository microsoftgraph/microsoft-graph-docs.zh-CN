# <a name="rangesort-apply"></a><span data-ttu-id="f8440-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="f8440-101">RangeSort: apply</span></span>

<span data-ttu-id="f8440-102">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="f8440-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8440-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8440-103">Prerequisites</span></span>
<span data-ttu-id="f8440-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="f8440-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="f8440-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8440-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="f8440-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8440-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="f8440-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8440-107">Request headers</span></span>
| <span data-ttu-id="f8440-108">名称</span><span class="sxs-lookup"><span data-stu-id="f8440-108">Name</span></span>       | <span data-ttu-id="f8440-109">说明</span><span class="sxs-lookup"><span data-stu-id="f8440-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8440-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8440-110">Authorization</span></span>  | <span data-ttu-id="f8440-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8440-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f8440-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8440-113">Request body</span></span>
<span data-ttu-id="f8440-114">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f8440-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8440-115">参数</span><span class="sxs-lookup"><span data-stu-id="f8440-115">Parameter</span></span>    | <span data-ttu-id="f8440-116">类型</span><span class="sxs-lookup"><span data-stu-id="f8440-116">Type</span></span>   |<span data-ttu-id="f8440-117">说明</span><span class="sxs-lookup"><span data-stu-id="f8440-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8440-118">fields</span><span class="sxs-lookup"><span data-stu-id="f8440-118">fields</span></span>|<span data-ttu-id="f8440-119">SortField</span><span class="sxs-lookup"><span data-stu-id="f8440-119">SortField</span></span>|<span data-ttu-id="f8440-120">作为排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="f8440-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="f8440-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="f8440-121">matchCase</span></span>|<span data-ttu-id="f8440-122">boolean</span><span class="sxs-lookup"><span data-stu-id="f8440-122">boolean</span></span>|<span data-ttu-id="f8440-p102">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="f8440-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="f8440-125">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="f8440-125">hasHeaders</span></span>|<span data-ttu-id="f8440-126">boolean</span><span class="sxs-lookup"><span data-stu-id="f8440-126">boolean</span></span>|<span data-ttu-id="f8440-p103">可选。该区域是否有标头。</span><span class="sxs-lookup"><span data-stu-id="f8440-p103">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="f8440-129">orientation</span><span class="sxs-lookup"><span data-stu-id="f8440-129">orientation</span></span>|<span data-ttu-id="f8440-130">string</span><span class="sxs-lookup"><span data-stu-id="f8440-130">string</span></span>|<span data-ttu-id="f8440-p104">可选。该操作是对行还是列排序。可能的值是：`Rows`、`Columns`。</span><span class="sxs-lookup"><span data-stu-id="f8440-p104">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="f8440-134">method</span><span class="sxs-lookup"><span data-stu-id="f8440-134">method</span></span>|<span data-ttu-id="f8440-135">string</span><span class="sxs-lookup"><span data-stu-id="f8440-135">string</span></span>|<span data-ttu-id="f8440-p105">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="f8440-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="f8440-139">响应</span><span class="sxs-lookup"><span data-stu-id="f8440-139">Response</span></span>

<span data-ttu-id="f8440-p106">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f8440-p106">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8440-142">示例</span><span class="sxs-lookup"><span data-stu-id="f8440-142">Example</span></span>
<span data-ttu-id="f8440-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f8440-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8440-144">请求</span><span class="sxs-lookup"><span data-stu-id="f8440-144">Request</span></span>
<span data-ttu-id="f8440-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8440-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="f8440-146">响应</span><span class="sxs-lookup"><span data-stu-id="f8440-146">Response</span></span>
<span data-ttu-id="f8440-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f8440-147">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->