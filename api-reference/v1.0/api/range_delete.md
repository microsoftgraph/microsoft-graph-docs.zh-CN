# <a name="range-delete"></a><span data-ttu-id="771d9-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="771d9-101">Range: delete</span></span>

<span data-ttu-id="771d9-102">删除与区域相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="771d9-102">Deletes the cells associated with the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="771d9-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="771d9-103">Prerequisites</span></span>
<span data-ttu-id="771d9-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="771d9-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="771d9-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="771d9-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="771d9-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="771d9-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="771d9-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="771d9-107">Request headers</span></span>
| <span data-ttu-id="771d9-108">名称</span><span class="sxs-lookup"><span data-stu-id="771d9-108">Name</span></span>       | <span data-ttu-id="771d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="771d9-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="771d9-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="771d9-110">Authorization</span></span>  | <span data-ttu-id="771d9-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="771d9-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="771d9-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="771d9-113">Request body</span></span>
<span data-ttu-id="771d9-114">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="771d9-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="771d9-115">参数</span><span class="sxs-lookup"><span data-stu-id="771d9-115">Parameter</span></span>    | <span data-ttu-id="771d9-116">类型</span><span class="sxs-lookup"><span data-stu-id="771d9-116">Type</span></span>   |<span data-ttu-id="771d9-117">说明</span><span class="sxs-lookup"><span data-stu-id="771d9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="771d9-118">Shift</span><span class="sxs-lookup"><span data-stu-id="771d9-118">shift</span></span>|<span data-ttu-id="771d9-119">string</span><span class="sxs-lookup"><span data-stu-id="771d9-119">string</span></span>|<span data-ttu-id="771d9-p102">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="771d9-p102">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="771d9-122">响应</span><span class="sxs-lookup"><span data-stu-id="771d9-122">Response</span></span>

<span data-ttu-id="771d9-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="771d9-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="771d9-125">示例</span><span class="sxs-lookup"><span data-stu-id="771d9-125">Example</span></span>
<span data-ttu-id="771d9-126">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="771d9-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="771d9-127">请求</span><span class="sxs-lookup"><span data-stu-id="771d9-127">Request</span></span>
<span data-ttu-id="771d9-128">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="771d9-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="771d9-129">响应</span><span class="sxs-lookup"><span data-stu-id="771d9-129">Response</span></span>
<span data-ttu-id="771d9-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="771d9-130">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->