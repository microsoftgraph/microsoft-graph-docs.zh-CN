# <a name="create-chartseries"></a><span data-ttu-id="e6be9-101">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e6be9-101">Create ChartSeries</span></span>

<span data-ttu-id="e6be9-102">使用此 API 创建新 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="e6be9-102">Use this API to create a new ChartSeries.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6be9-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6be9-103">Prerequisites</span></span>
<span data-ttu-id="e6be9-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="e6be9-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e6be9-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6be9-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e6be9-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6be9-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="e6be9-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6be9-107">Request headers</span></span>
| <span data-ttu-id="e6be9-108">名称</span><span class="sxs-lookup"><span data-stu-id="e6be9-108">Name</span></span>       | <span data-ttu-id="e6be9-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6be9-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6be9-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6be9-110">Authorization</span></span>  | <span data-ttu-id="e6be9-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6be9-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e6be9-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6be9-113">Request body</span></span>
<span data-ttu-id="e6be9-114">在请求正文中，提供 [ChartSeries](../resources/chartseries.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6be9-114">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e6be9-115">响应</span><span class="sxs-lookup"><span data-stu-id="e6be9-115">Response</span></span>

<span data-ttu-id="e6be9-116">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [ChartSeries](../resources/chartseries.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6be9-116">If successful, this method returns `201, Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6be9-117">示例</span><span class="sxs-lookup"><span data-stu-id="e6be9-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6be9-118">请求</span><span class="sxs-lookup"><span data-stu-id="e6be9-118">Request</span></span>
<span data-ttu-id="e6be9-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6be9-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="e6be9-120">在请求正文中，提供 [ChartSeries](../resources/chartseries.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6be9-120">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6be9-121">响应</span><span class="sxs-lookup"><span data-stu-id="e6be9-121">Response</span></span>
<span data-ttu-id="e6be9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6be9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->