# <a name="chartpointscollection-itemat"></a><span data-ttu-id="d57fa-101">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="d57fa-101">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="d57fa-102">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="d57fa-102">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="d57fa-103">权限</span><span class="sxs-lookup"><span data-stu-id="d57fa-103">Permissions</span></span>
<span data-ttu-id="d57fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d57fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d57fa-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d57fa-106">Permission type</span></span>      | <span data-ttu-id="d57fa-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d57fa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d57fa-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d57fa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d57fa-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d57fa-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d57fa-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d57fa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d57fa-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d57fa-111">Not supported.</span></span>    |
|<span data-ttu-id="d57fa-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d57fa-112">Application</span></span> | <span data-ttu-id="d57fa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d57fa-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d57fa-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d57fa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="d57fa-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="d57fa-115">Request headers</span></span>
| <span data-ttu-id="d57fa-116">名称</span><span class="sxs-lookup"><span data-stu-id="d57fa-116">Name</span></span>       | <span data-ttu-id="d57fa-117">说明</span><span class="sxs-lookup"><span data-stu-id="d57fa-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d57fa-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d57fa-118">Authorization</span></span>  | <span data-ttu-id="d57fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d57fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d57fa-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="d57fa-121">Request body</span></span>
<span data-ttu-id="d57fa-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d57fa-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d57fa-123">参数</span><span class="sxs-lookup"><span data-stu-id="d57fa-123">Parameter</span></span>    | <span data-ttu-id="d57fa-124">类型</span><span class="sxs-lookup"><span data-stu-id="d57fa-124">Type</span></span>   |<span data-ttu-id="d57fa-125">说明</span><span class="sxs-lookup"><span data-stu-id="d57fa-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d57fa-126">index</span><span class="sxs-lookup"><span data-stu-id="d57fa-126">index</span></span>|<span data-ttu-id="d57fa-127">number</span><span class="sxs-lookup"><span data-stu-id="d57fa-127">number</span></span>|<span data-ttu-id="d57fa-p103">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="d57fa-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="d57fa-130">响应</span><span class="sxs-lookup"><span data-stu-id="d57fa-130">Response</span></span>

<span data-ttu-id="d57fa-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ChartPoint](../resources/chartpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d57fa-131">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d57fa-132">示例</span><span class="sxs-lookup"><span data-stu-id="d57fa-132">Example</span></span>
<span data-ttu-id="d57fa-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d57fa-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d57fa-134">请求</span><span class="sxs-lookup"><span data-stu-id="d57fa-134">Request</span></span>
<span data-ttu-id="d57fa-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d57fa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="d57fa-136">响应</span><span class="sxs-lookup"><span data-stu-id="d57fa-136">Response</span></span>
<span data-ttu-id="d57fa-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d57fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->