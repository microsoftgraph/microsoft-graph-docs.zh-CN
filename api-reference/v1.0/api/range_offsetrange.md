# <a name="range-offsetrange"></a><span data-ttu-id="ab468-101">Range:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="ab468-101">Range: OffsetRange</span></span>

<span data-ttu-id="ab468-p101">获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。</span><span class="sxs-lookup"><span data-stu-id="ab468-p101">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab468-105">权限</span><span class="sxs-lookup"><span data-stu-id="ab468-105">Permissions</span></span>
<span data-ttu-id="ab468-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ab468-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab468-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab468-108">Permission type</span></span>      | <span data-ttu-id="ab468-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab468-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab468-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab468-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab468-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab468-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab468-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab468-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab468-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab468-113">Not supported.</span></span>    |
|<span data-ttu-id="ab468-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab468-114">Application</span></span> | <span data-ttu-id="ab468-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab468-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab468-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab468-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="ab468-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab468-117">Request headers</span></span>
| <span data-ttu-id="ab468-118">名称</span><span class="sxs-lookup"><span data-stu-id="ab468-118">Name</span></span>       | <span data-ttu-id="ab468-119">说明</span><span class="sxs-lookup"><span data-stu-id="ab468-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab468-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab468-120">Authorization</span></span>  | <span data-ttu-id="ab468-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab468-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab468-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab468-123">Request body</span></span>
<span data-ttu-id="ab468-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ab468-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ab468-125">参数</span><span class="sxs-lookup"><span data-stu-id="ab468-125">Parameter</span></span>    | <span data-ttu-id="ab468-126">类型</span><span class="sxs-lookup"><span data-stu-id="ab468-126">Type</span></span>   |<span data-ttu-id="ab468-127">说明</span><span class="sxs-lookup"><span data-stu-id="ab468-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab468-128">rowOffset</span><span class="sxs-lookup"><span data-stu-id="ab468-128">rowOffset</span></span>|<span data-ttu-id="ab468-129">number</span><span class="sxs-lookup"><span data-stu-id="ab468-129">number</span></span>|<span data-ttu-id="ab468-p104">区域偏移的行数（正数、负数或 0）。正数表示向下偏移，负数表示向上偏移。</span><span class="sxs-lookup"><span data-stu-id="ab468-p104">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="ab468-132">columnOffset</span><span class="sxs-lookup"><span data-stu-id="ab468-132">columnOffset</span></span>|<span data-ttu-id="ab468-133">number</span><span class="sxs-lookup"><span data-stu-id="ab468-133">number</span></span>|<span data-ttu-id="ab468-p105">区域偏移的列数（正数、负数或 0）。正数表示向右偏移，负数表示向左偏移。</span><span class="sxs-lookup"><span data-stu-id="ab468-p105">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="ab468-136">响应</span><span class="sxs-lookup"><span data-stu-id="ab468-136">Response</span></span>

<span data-ttu-id="ab468-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab468-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab468-138">示例</span><span class="sxs-lookup"><span data-stu-id="ab468-138">Example</span></span>
<span data-ttu-id="ab468-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ab468-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab468-140">请求</span><span class="sxs-lookup"><span data-stu-id="ab468-140">Request</span></span>
<span data-ttu-id="ab468-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab468-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="ab468-142">响应</span><span class="sxs-lookup"><span data-stu-id="ab468-142">Response</span></span>
<span data-ttu-id="ab468-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab468-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->