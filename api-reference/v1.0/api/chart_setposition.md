# <a name="chart-setposition"></a><span data-ttu-id="920d3-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="920d3-101">Chart: setPosition</span></span>

<span data-ttu-id="920d3-102">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="920d3-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="920d3-103">权限</span><span class="sxs-lookup"><span data-stu-id="920d3-103">Permissions</span></span>
<span data-ttu-id="920d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="920d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="920d3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="920d3-106">Permission type</span></span>      | <span data-ttu-id="920d3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="920d3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="920d3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="920d3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="920d3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="920d3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="920d3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="920d3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="920d3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="920d3-111">Not supported.</span></span>    |
|<span data-ttu-id="920d3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="920d3-112">Application</span></span> | <span data-ttu-id="920d3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="920d3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="920d3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="920d3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="920d3-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="920d3-115">Request headers</span></span>
| <span data-ttu-id="920d3-116">名称</span><span class="sxs-lookup"><span data-stu-id="920d3-116">Name</span></span>       | <span data-ttu-id="920d3-117">说明</span><span class="sxs-lookup"><span data-stu-id="920d3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="920d3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="920d3-118">Authorization</span></span>  | <span data-ttu-id="920d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="920d3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="920d3-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="920d3-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="920d3-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="920d3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="920d3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="920d3-124">Request body</span></span>
<span data-ttu-id="920d3-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="920d3-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="920d3-126">参数</span><span class="sxs-lookup"><span data-stu-id="920d3-126">Parameter</span></span>    | <span data-ttu-id="920d3-127">类型</span><span class="sxs-lookup"><span data-stu-id="920d3-127">Type</span></span>   |<span data-ttu-id="920d3-128">说明</span><span class="sxs-lookup"><span data-stu-id="920d3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="920d3-129">startCell</span><span class="sxs-lookup"><span data-stu-id="920d3-129">startCell</span></span>|<span data-ttu-id="920d3-130">string</span><span class="sxs-lookup"><span data-stu-id="920d3-130">string</span></span>|<span data-ttu-id="920d3-p104">起始单元格。这是图表将移动到的位置。起始单元格为左上角或右上角的单元格，具体取决于用户的从右到左显示设置。</span><span class="sxs-lookup"><span data-stu-id="920d3-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="920d3-134">endCell</span><span class="sxs-lookup"><span data-stu-id="920d3-134">endCell</span></span>|<span data-ttu-id="920d3-135">string</span><span class="sxs-lookup"><span data-stu-id="920d3-135">string</span></span>|<span data-ttu-id="920d3-p105">可选。结束单元格。如果已指定，图表的宽度和高度将设置为完全覆盖此单元格/区域。</span><span class="sxs-lookup"><span data-stu-id="920d3-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="920d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="920d3-139">Response</span></span>

<span data-ttu-id="920d3-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="920d3-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="920d3-142">示例</span><span class="sxs-lookup"><span data-stu-id="920d3-142">Example</span></span>
<span data-ttu-id="920d3-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="920d3-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="920d3-144">请求</span><span class="sxs-lookup"><span data-stu-id="920d3-144">Request</span></span>
<span data-ttu-id="920d3-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="920d3-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="920d3-146">响应</span><span class="sxs-lookup"><span data-stu-id="920d3-146">Response</span></span>
<span data-ttu-id="920d3-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="920d3-147">Here is an example of the response.</span></span> 
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
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->