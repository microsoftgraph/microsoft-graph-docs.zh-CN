# <a name="tablesort-apply"></a><span data-ttu-id="5739a-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="5739a-101">TableSort: apply</span></span>

<span data-ttu-id="5739a-102">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="5739a-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="5739a-103">权限</span><span class="sxs-lookup"><span data-stu-id="5739a-103">Permissions</span></span>
<span data-ttu-id="5739a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5739a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5739a-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="5739a-106">Permission type</span></span>      | <span data-ttu-id="5739a-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5739a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5739a-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5739a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5739a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5739a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5739a-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5739a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5739a-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="5739a-111">Not supported.</span></span>    |
|<span data-ttu-id="5739a-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="5739a-112">Application</span></span> | <span data-ttu-id="5739a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5739a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5739a-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5739a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="5739a-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="5739a-115">Request headers</span></span>
| <span data-ttu-id="5739a-116">名称</span><span class="sxs-lookup"><span data-stu-id="5739a-116">Name</span></span>       | <span data-ttu-id="5739a-117">说明</span><span class="sxs-lookup"><span data-stu-id="5739a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5739a-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="5739a-118">Authorization</span></span>  | <span data-ttu-id="5739a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5739a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5739a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5739a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="5739a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5739a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5739a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5739a-124">Request body</span></span>
<span data-ttu-id="5739a-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5739a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5739a-126">参数</span><span class="sxs-lookup"><span data-stu-id="5739a-126">Parameter</span></span>    | <span data-ttu-id="5739a-127">类型</span><span class="sxs-lookup"><span data-stu-id="5739a-127">Type</span></span>   |<span data-ttu-id="5739a-128">说明</span><span class="sxs-lookup"><span data-stu-id="5739a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5739a-129">fields</span><span class="sxs-lookup"><span data-stu-id="5739a-129">fields</span></span>|<span data-ttu-id="5739a-130">SortField</span><span class="sxs-lookup"><span data-stu-id="5739a-130">SortField</span></span>|<span data-ttu-id="5739a-131">作为排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="5739a-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="5739a-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="5739a-132">matchCase</span></span>|<span data-ttu-id="5739a-133">布尔</span><span class="sxs-lookup"><span data-stu-id="5739a-133">boolean</span></span>|<span data-ttu-id="5739a-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="5739a-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="5739a-136">method</span><span class="sxs-lookup"><span data-stu-id="5739a-136">method</span></span>|<span data-ttu-id="5739a-137">string</span><span class="sxs-lookup"><span data-stu-id="5739a-137">string</span></span>|<span data-ttu-id="5739a-p105">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="5739a-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="5739a-141">响应</span><span class="sxs-lookup"><span data-stu-id="5739a-141">Response</span></span>

<span data-ttu-id="5739a-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5739a-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5739a-144">示例</span><span class="sxs-lookup"><span data-stu-id="5739a-144">Example</span></span>
<span data-ttu-id="5739a-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5739a-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5739a-146">请求</span><span class="sxs-lookup"><span data-stu-id="5739a-146">Request</span></span>
<span data-ttu-id="5739a-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5739a-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5739a-148">响应</span><span class="sxs-lookup"><span data-stu-id="5739a-148">Response</span></span>
<span data-ttu-id="5739a-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5739a-149">Here is an example of the response.</span></span> 
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