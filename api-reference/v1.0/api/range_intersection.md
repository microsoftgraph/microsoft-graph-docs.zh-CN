# <a name="range-intersection"></a><span data-ttu-id="c7c7d-101">Range:Intersection</span><span class="sxs-lookup"><span data-stu-id="c7c7d-101">Range: Intersection</span></span>

<span data-ttu-id="c7c7d-102">获取表示给定范围的矩形交集的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7c7d-103">权限</span><span class="sxs-lookup"><span data-stu-id="c7c7d-103">Permissions</span></span>
<span data-ttu-id="c7c7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7c7d-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7c7d-106">Permission type</span></span>      | <span data-ttu-id="c7c7d-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7c7d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c7d-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c7d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c7c7d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c7d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7c7d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c7d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c7d-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-111">Not supported.</span></span>    |
|<span data-ttu-id="c7c7d-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7c7d-112">Application</span></span> | <span data-ttu-id="c7c7d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c7d-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7c7d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="c7c7d-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7c7d-115">Request headers</span></span>
| <span data-ttu-id="c7c7d-116">名称</span><span class="sxs-lookup"><span data-stu-id="c7c7d-116">Name</span></span>       | <span data-ttu-id="c7c7d-117">说明</span><span class="sxs-lookup"><span data-stu-id="c7c7d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7c7d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c7d-118">Authorization</span></span>  | <span data-ttu-id="c7c7d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7c7d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c7c7d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7c7d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c7d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7c7d-124">Request body</span></span>
<span data-ttu-id="c7c7d-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7c7d-126">参数</span><span class="sxs-lookup"><span data-stu-id="c7c7d-126">Parameter</span></span>    | <span data-ttu-id="c7c7d-127">类型</span><span class="sxs-lookup"><span data-stu-id="c7c7d-127">Type</span></span>   |<span data-ttu-id="c7c7d-128">说明</span><span class="sxs-lookup"><span data-stu-id="c7c7d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7c7d-129">anotherRange</span><span class="sxs-lookup"><span data-stu-id="c7c7d-129">anotherRange</span></span>|<span data-ttu-id="c7c7d-130">string</span><span class="sxs-lookup"><span data-stu-id="c7c7d-130">string</span></span>|<span data-ttu-id="c7c7d-131">将用于确定区域交集的 range 对象或区域地址。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-131">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="c7c7d-132">响应</span><span class="sxs-lookup"><span data-stu-id="c7c7d-132">Response</span></span>

<span data-ttu-id="c7c7d-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-133">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c7d-134">示例</span><span class="sxs-lookup"><span data-stu-id="c7c7d-134">Example</span></span>
<span data-ttu-id="c7c7d-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7c7d-136">请求</span><span class="sxs-lookup"><span data-stu-id="c7c7d-136">Request</span></span>
<span data-ttu-id="c7c7d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="c7c7d-138">响应</span><span class="sxs-lookup"><span data-stu-id="c7c7d-138">Response</span></span>
<span data-ttu-id="c7c7d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7c7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->