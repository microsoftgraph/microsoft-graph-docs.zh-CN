# <a name="worksheet-cell"></a><span data-ttu-id="407ab-101">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="407ab-101">Worksheet: Cell</span></span>

<span data-ttu-id="407ab-p101">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="407ab-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="407ab-104">权限</span><span class="sxs-lookup"><span data-stu-id="407ab-104">Permissions</span></span>
<span data-ttu-id="407ab-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="407ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="407ab-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="407ab-107">Permission type</span></span>      | <span data-ttu-id="407ab-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="407ab-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="407ab-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="407ab-109">Delegated (work or school account)</span></span> | <span data-ttu-id="407ab-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="407ab-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="407ab-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="407ab-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="407ab-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="407ab-112">Not supported.</span></span>    |
|<span data-ttu-id="407ab-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="407ab-113">Application</span></span> | <span data-ttu-id="407ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="407ab-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="407ab-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="407ab-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="407ab-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="407ab-116">Request headers</span></span>
| <span data-ttu-id="407ab-117">名称</span><span class="sxs-lookup"><span data-stu-id="407ab-117">Name</span></span>       | <span data-ttu-id="407ab-118">说明</span><span class="sxs-lookup"><span data-stu-id="407ab-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="407ab-119">授权</span><span class="sxs-lookup"><span data-stu-id="407ab-119">Authorization</span></span>  | <span data-ttu-id="407ab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="407ab-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="407ab-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="407ab-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="407ab-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="407ab-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="407ab-125">参数</span><span class="sxs-lookup"><span data-stu-id="407ab-125">Parameters</span></span>
<span data-ttu-id="407ab-126">在请求路径中，提供了以下参数。</span><span class="sxs-lookup"><span data-stu-id="407ab-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="407ab-127">参数</span><span class="sxs-lookup"><span data-stu-id="407ab-127">Parameter</span></span>    | <span data-ttu-id="407ab-128">类型</span><span class="sxs-lookup"><span data-stu-id="407ab-128">Type</span></span>   |<span data-ttu-id="407ab-129">说明</span><span class="sxs-lookup"><span data-stu-id="407ab-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="407ab-130">row</span><span class="sxs-lookup"><span data-stu-id="407ab-130">row</span></span>|<span data-ttu-id="407ab-131">Int32</span><span class="sxs-lookup"><span data-stu-id="407ab-131">Int32</span></span>|<span data-ttu-id="407ab-p105">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="407ab-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="407ab-134">列</span><span class="sxs-lookup"><span data-stu-id="407ab-134">column</span></span>|<span data-ttu-id="407ab-135">Int32</span><span class="sxs-lookup"><span data-stu-id="407ab-135">Int32</span></span>|<span data-ttu-id="407ab-p106">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="407ab-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="407ab-138">响应</span><span class="sxs-lookup"><span data-stu-id="407ab-138">Response</span></span>

<span data-ttu-id="407ab-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="407ab-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="407ab-140">示例</span><span class="sxs-lookup"><span data-stu-id="407ab-140">Example</span></span>
<span data-ttu-id="407ab-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="407ab-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="407ab-142">请求</span><span class="sxs-lookup"><span data-stu-id="407ab-142">Request</span></span>
<span data-ttu-id="407ab-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="407ab-143">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="407ab-144">响应</span><span class="sxs-lookup"><span data-stu-id="407ab-144">Response</span></span>
<span data-ttu-id="407ab-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="407ab-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
