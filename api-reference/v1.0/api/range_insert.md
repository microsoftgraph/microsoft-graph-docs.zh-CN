# <a name="range-insert"></a><span data-ttu-id="33fa8-101">Range: insert</span><span class="sxs-lookup"><span data-stu-id="33fa8-101">Range: insert</span></span>

<span data-ttu-id="33fa8-p101">将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="33fa8-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="33fa8-104">权限</span><span class="sxs-lookup"><span data-stu-id="33fa8-104">Permissions</span></span>
<span data-ttu-id="33fa8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="33fa8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="33fa8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="33fa8-107">Permission type</span></span>      | <span data-ttu-id="33fa8-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33fa8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33fa8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33fa8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="33fa8-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33fa8-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33fa8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33fa8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33fa8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="33fa8-112">Not supported.</span></span>    |
|<span data-ttu-id="33fa8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="33fa8-113">Application</span></span> | <span data-ttu-id="33fa8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33fa8-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33fa8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33fa8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(<address>)/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="33fa8-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="33fa8-116">Request headers</span></span>
| <span data-ttu-id="33fa8-117">名称</span><span class="sxs-lookup"><span data-stu-id="33fa8-117">Name</span></span>       | <span data-ttu-id="33fa8-118">说明</span><span class="sxs-lookup"><span data-stu-id="33fa8-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="33fa8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="33fa8-119">Authorization</span></span>  | <span data-ttu-id="33fa8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33fa8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33fa8-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="33fa8-122">Request body</span></span>
<span data-ttu-id="33fa8-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="33fa8-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33fa8-124">参数</span><span class="sxs-lookup"><span data-stu-id="33fa8-124">Parameter</span></span>    | <span data-ttu-id="33fa8-125">类型</span><span class="sxs-lookup"><span data-stu-id="33fa8-125">Type</span></span>   |<span data-ttu-id="33fa8-126">说明</span><span class="sxs-lookup"><span data-stu-id="33fa8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33fa8-127">Shift</span><span class="sxs-lookup"><span data-stu-id="33fa8-127">shift</span></span>|<span data-ttu-id="33fa8-128">string</span><span class="sxs-lookup"><span data-stu-id="33fa8-128">string</span></span>|<span data-ttu-id="33fa8-p104">指定移动单元格的方式。可能的值是：`Down`、`Right`。</span><span class="sxs-lookup"><span data-stu-id="33fa8-p104">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="33fa8-131">响应</span><span class="sxs-lookup"><span data-stu-id="33fa8-131">Response</span></span>

<span data-ttu-id="33fa8-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33fa8-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33fa8-133">示例</span><span class="sxs-lookup"><span data-stu-id="33fa8-133">Example</span></span>
<span data-ttu-id="33fa8-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="33fa8-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33fa8-135">请求</span><span class="sxs-lookup"><span data-stu-id="33fa8-135">Request</span></span>
<span data-ttu-id="33fa8-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33fa8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="33fa8-137">响应</span><span class="sxs-lookup"><span data-stu-id="33fa8-137">Response</span></span>
<span data-ttu-id="33fa8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33fa8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->