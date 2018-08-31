# <a name="worksheet-range"></a><span data-ttu-id="994e7-101">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="994e7-101">Worksheet: Range</span></span>

<span data-ttu-id="994e7-102">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="994e7-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="994e7-103">权限</span><span class="sxs-lookup"><span data-stu-id="994e7-103">Permissions</span></span>
<span data-ttu-id="994e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="994e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="994e7-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="994e7-106">Permission type</span></span>      | <span data-ttu-id="994e7-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="994e7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="994e7-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="994e7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="994e7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="994e7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="994e7-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="994e7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994e7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="994e7-111">Not supported.</span></span>    |
|<span data-ttu-id="994e7-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="994e7-112">Application</span></span> | <span data-ttu-id="994e7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="994e7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="994e7-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="994e7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="994e7-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="994e7-115">Request headers</span></span>
| <span data-ttu-id="994e7-116">名称</span><span class="sxs-lookup"><span data-stu-id="994e7-116">Name</span></span>       | <span data-ttu-id="994e7-117">说明</span><span class="sxs-lookup"><span data-stu-id="994e7-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="994e7-118">授权</span><span class="sxs-lookup"><span data-stu-id="994e7-118">Authorization</span></span>  | <span data-ttu-id="994e7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="994e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="994e7-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="994e7-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="994e7-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="994e7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="994e7-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="994e7-124">Function parameters</span></span>

| <span data-ttu-id="994e7-125">参数</span><span class="sxs-lookup"><span data-stu-id="994e7-125">Parameter</span></span>    | <span data-ttu-id="994e7-126">类型</span><span class="sxs-lookup"><span data-stu-id="994e7-126">Type</span></span>   |<span data-ttu-id="994e7-127">说明</span><span class="sxs-lookup"><span data-stu-id="994e7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="994e7-128">address</span><span class="sxs-lookup"><span data-stu-id="994e7-128">address</span></span>|<span data-ttu-id="994e7-129">string</span><span class="sxs-lookup"><span data-stu-id="994e7-129">string</span></span>|<span data-ttu-id="994e7-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="994e7-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="994e7-133">响应</span><span class="sxs-lookup"><span data-stu-id="994e7-133">Response</span></span>

<span data-ttu-id="994e7-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="994e7-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="994e7-135">示例</span><span class="sxs-lookup"><span data-stu-id="994e7-135">Example</span></span>
<span data-ttu-id="994e7-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="994e7-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="994e7-137">请求</span><span class="sxs-lookup"><span data-stu-id="994e7-137">Request</span></span>
<span data-ttu-id="994e7-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="994e7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="994e7-139">响应</span><span class="sxs-lookup"><span data-stu-id="994e7-139">Response</span></span>
<span data-ttu-id="994e7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="994e7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<span data-ttu-id="994e7-143">如果未指定可选 `address` 参数，此函数将返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="994e7-143">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="994e7-144">请求</span><span class="sxs-lookup"><span data-stu-id="994e7-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="994e7-145">响应</span><span class="sxs-lookup"><span data-stu-id="994e7-145">Response</span></span>

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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->