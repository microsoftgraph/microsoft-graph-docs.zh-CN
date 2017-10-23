# <a name="worksheet-cell"></a><span data-ttu-id="a1d51-101">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="a1d51-101">Worksheet: Cell</span></span>

<span data-ttu-id="a1d51-p101">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="a1d51-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1d51-104">权限</span><span class="sxs-lookup"><span data-stu-id="a1d51-104">Permissions</span></span>
<span data-ttu-id="a1d51-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a1d51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1d51-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1d51-107">Permission type</span></span>      | <span data-ttu-id="a1d51-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1d51-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1d51-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1d51-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a1d51-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1d51-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a1d51-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1d51-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1d51-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1d51-112">Not supported.</span></span>    |
|<span data-ttu-id="a1d51-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1d51-113">Application</span></span> | <span data-ttu-id="a1d51-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1d51-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1d51-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1d51-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="a1d51-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1d51-116">Request headers</span></span>
| <span data-ttu-id="a1d51-117">名称</span><span class="sxs-lookup"><span data-stu-id="a1d51-117">Name</span></span>       | <span data-ttu-id="a1d51-118">说明</span><span class="sxs-lookup"><span data-stu-id="a1d51-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1d51-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1d51-119">Authorization</span></span>  | <span data-ttu-id="a1d51-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1d51-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a1d51-122">响应</span><span class="sxs-lookup"><span data-stu-id="a1d51-122">Response</span></span>

<span data-ttu-id="a1d51-123">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1d51-123">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1d51-124">示例</span><span class="sxs-lookup"><span data-stu-id="a1d51-124">Example</span></span>
<span data-ttu-id="a1d51-125">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a1d51-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a1d51-126">请求</span><span class="sxs-lookup"><span data-stu-id="a1d51-126">Request</span></span>
<span data-ttu-id="a1d51-127">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1d51-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="a1d51-128">响应</span><span class="sxs-lookup"><span data-stu-id="a1d51-128">Response</span></span>
<span data-ttu-id="a1d51-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1d51-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
