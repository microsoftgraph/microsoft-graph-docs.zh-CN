# <a name="worksheet-usedrange"></a><span data-ttu-id="2514e-101">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="2514e-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="2514e-p101">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="2514e-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="2514e-104">权限</span><span class="sxs-lookup"><span data-stu-id="2514e-104">Permissions</span></span>
<span data-ttu-id="2514e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2514e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2514e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2514e-107">Permission type</span></span>      | <span data-ttu-id="2514e-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2514e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2514e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2514e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2514e-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2514e-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2514e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2514e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2514e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2514e-112">Not supported.</span></span>    |
|<span data-ttu-id="2514e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2514e-113">Application</span></span> | <span data-ttu-id="2514e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2514e-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2514e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2514e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="2514e-116">可选的请求参数</span><span class="sxs-lookup"><span data-stu-id="2514e-116">Optional request parameter</span></span>
<span data-ttu-id="2514e-117">在请求 URL 中，提供可选的查询参数。</span><span class="sxs-lookup"><span data-stu-id="2514e-117">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="2514e-118">参数</span><span class="sxs-lookup"><span data-stu-id="2514e-118">Parameter</span></span>    | <span data-ttu-id="2514e-119">类型</span><span class="sxs-lookup"><span data-stu-id="2514e-119">Type</span></span>   |<span data-ttu-id="2514e-120">说明</span><span class="sxs-lookup"><span data-stu-id="2514e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2514e-121">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="2514e-121">valuesOnly</span></span>|<span data-ttu-id="2514e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="2514e-122">Boolean</span></span>|<span data-ttu-id="2514e-p103">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="2514e-p103">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2514e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="2514e-125">Request headers</span></span>
| <span data-ttu-id="2514e-126">名称</span><span class="sxs-lookup"><span data-stu-id="2514e-126">Name</span></span>       | <span data-ttu-id="2514e-127">说明</span><span class="sxs-lookup"><span data-stu-id="2514e-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2514e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2514e-128">Authorization</span></span>  | <span data-ttu-id="2514e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2514e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2514e-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2514e-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="2514e-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2514e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="2514e-134">响应</span><span class="sxs-lookup"><span data-stu-id="2514e-134">Response</span></span>

<span data-ttu-id="2514e-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2514e-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2514e-136">示例</span><span class="sxs-lookup"><span data-stu-id="2514e-136">Example</span></span>
<span data-ttu-id="2514e-137">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2514e-137">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2514e-138">请求</span><span class="sxs-lookup"><span data-stu-id="2514e-138">Request</span></span>
<span data-ttu-id="2514e-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2514e-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="2514e-140">响应</span><span class="sxs-lookup"><span data-stu-id="2514e-140">Response</span></span>
<span data-ttu-id="2514e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2514e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
