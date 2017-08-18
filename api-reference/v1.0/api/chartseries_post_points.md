# <a name="create-chartpoints"></a><span data-ttu-id="2af56-101">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="2af56-101">Create ChartPoints</span></span>

<span data-ttu-id="2af56-102">使用此 API 创建新 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="2af56-102">Use this API to create a new ChartPoints.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2af56-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="2af56-103">Prerequisites</span></span>
<span data-ttu-id="2af56-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="2af56-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="2af56-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2af56-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="2af56-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2af56-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="2af56-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="2af56-107">Request headers</span></span>
| <span data-ttu-id="2af56-108">名称</span><span class="sxs-lookup"><span data-stu-id="2af56-108">Name</span></span>       | <span data-ttu-id="2af56-109">说明</span><span class="sxs-lookup"><span data-stu-id="2af56-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2af56-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af56-110">Authorization</span></span>  | <span data-ttu-id="2af56-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2af56-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2af56-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="2af56-113">Request body</span></span>
<span data-ttu-id="2af56-114">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2af56-114">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2af56-115">响应</span><span class="sxs-lookup"><span data-stu-id="2af56-115">Response</span></span>

<span data-ttu-id="2af56-116">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [ChartPoints](../resources/chartpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2af56-116">If successful, this method returns `201, Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2af56-117">示例</span><span class="sxs-lookup"><span data-stu-id="2af56-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2af56-118">请求</span><span class="sxs-lookup"><span data-stu-id="2af56-118">Request</span></span>
<span data-ttu-id="2af56-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2af56-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="2af56-120">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2af56-120">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2af56-121">响应</span><span class="sxs-lookup"><span data-stu-id="2af56-121">Response</span></span>
<span data-ttu-id="2af56-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2af56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->