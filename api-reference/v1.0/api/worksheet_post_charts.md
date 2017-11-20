# <a name="create-chart"></a><span data-ttu-id="bb826-101">创建图表</span><span class="sxs-lookup"><span data-stu-id="bb826-101">Create Chart</span></span>

<span data-ttu-id="bb826-102">使用此 API 创建新图表。</span><span class="sxs-lookup"><span data-stu-id="bb826-102">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb826-103">权限</span><span class="sxs-lookup"><span data-stu-id="bb826-103">Permissions</span></span>
<span data-ttu-id="bb826-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bb826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bb826-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb826-106">Permission type</span></span>      | <span data-ttu-id="bb826-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb826-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb826-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb826-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bb826-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb826-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb826-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb826-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb826-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb826-111">Not supported.</span></span>    |
|<span data-ttu-id="bb826-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb826-112">Application</span></span> | <span data-ttu-id="bb826-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb826-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb826-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb826-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="bb826-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb826-115">Request headers</span></span>
| <span data-ttu-id="bb826-116">名称</span><span class="sxs-lookup"><span data-stu-id="bb826-116">Name</span></span>       | <span data-ttu-id="bb826-117">说明</span><span class="sxs-lookup"><span data-stu-id="bb826-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb826-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb826-118">Authorization</span></span>  | <span data-ttu-id="bb826-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb826-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb826-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bb826-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb826-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bb826-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb826-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb826-124">Request body</span></span>
<span data-ttu-id="bb826-125">在请求正文中，提供 [Chart](../resources/chart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb826-125">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bb826-126">响应</span><span class="sxs-lookup"><span data-stu-id="bb826-126">Response</span></span>

<span data-ttu-id="bb826-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb826-127">If successful, this method returns `201 Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb826-128">示例</span><span class="sxs-lookup"><span data-stu-id="bb826-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb826-129">请求</span><span class="sxs-lookup"><span data-stu-id="bb826-129">Request</span></span>
<span data-ttu-id="bb826-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb826-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="bb826-131">在请求正文中，提供 [Chart](../resources/chart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb826-131">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bb826-132">响应</span><span class="sxs-lookup"><span data-stu-id="bb826-132">Response</span></span>
<span data-ttu-id="bb826-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb826-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->