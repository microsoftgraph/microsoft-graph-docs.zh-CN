# <a name="chartseriescollection-itemat"></a><span data-ttu-id="0dfdd-101">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="0dfdd-101">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="0dfdd-102">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="0dfdd-102">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="0dfdd-103">权限</span><span class="sxs-lookup"><span data-stu-id="0dfdd-103">Permissions</span></span>
<span data-ttu-id="0dfdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0dfdd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dfdd-106">Permission type</span></span>      | <span data-ttu-id="0dfdd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0dfdd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dfdd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dfdd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0dfdd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfdd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0dfdd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dfdd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dfdd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-111">Not supported.</span></span>    |
|<span data-ttu-id="0dfdd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="0dfdd-112">Application</span></span> | <span data-ttu-id="0dfdd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dfdd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dfdd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="0dfdd-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dfdd-115">Request headers</span></span>
| <span data-ttu-id="0dfdd-116">名称</span><span class="sxs-lookup"><span data-stu-id="0dfdd-116">Name</span></span>       | <span data-ttu-id="0dfdd-117">说明</span><span class="sxs-lookup"><span data-stu-id="0dfdd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0dfdd-118">授权</span><span class="sxs-lookup"><span data-stu-id="0dfdd-118">Authorization</span></span>  | <span data-ttu-id="0dfdd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0dfdd-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0dfdd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="0dfdd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dfdd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dfdd-124">Request body</span></span>
<span data-ttu-id="0dfdd-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0dfdd-126">参数</span><span class="sxs-lookup"><span data-stu-id="0dfdd-126">Parameter</span></span>    | <span data-ttu-id="0dfdd-127">类型</span><span class="sxs-lookup"><span data-stu-id="0dfdd-127">Type</span></span>   |<span data-ttu-id="0dfdd-128">说明</span><span class="sxs-lookup"><span data-stu-id="0dfdd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0dfdd-129">index</span><span class="sxs-lookup"><span data-stu-id="0dfdd-129">index</span></span>|<span data-ttu-id="0dfdd-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfdd-130">Int32</span></span>|<span data-ttu-id="0dfdd-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0dfdd-133">响应</span><span class="sxs-lookup"><span data-stu-id="0dfdd-133">Response</span></span>

<span data-ttu-id="0dfdd-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [WorkbookChartSeries](../resources/chartseries.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dfdd-135">示例</span><span class="sxs-lookup"><span data-stu-id="0dfdd-135">Example</span></span>
<span data-ttu-id="0dfdd-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0dfdd-137">请求</span><span class="sxs-lookup"><span data-stu-id="0dfdd-137">Request</span></span>
<span data-ttu-id="0dfdd-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="0dfdd-139">响应</span><span class="sxs-lookup"><span data-stu-id="0dfdd-139">Response</span></span>
<span data-ttu-id="0dfdd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0dfdd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->