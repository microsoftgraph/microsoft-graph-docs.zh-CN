# <a name="create-chartpoints"></a><span data-ttu-id="ddeca-101">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="ddeca-101">Create ChartPoints</span></span>

<span data-ttu-id="ddeca-102">使用此 API 创建新 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="ddeca-102">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddeca-103">权限</span><span class="sxs-lookup"><span data-stu-id="ddeca-103">Permissions</span></span>
<span data-ttu-id="ddeca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ddeca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ddeca-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddeca-106">Permission type</span></span>      | <span data-ttu-id="ddeca-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddeca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddeca-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddeca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ddeca-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddeca-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddeca-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddeca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddeca-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddeca-111">Not supported.</span></span>    |
|<span data-ttu-id="ddeca-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddeca-112">Application</span></span> | <span data-ttu-id="ddeca-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddeca-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddeca-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddeca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="ddeca-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddeca-115">Request headers</span></span>
| <span data-ttu-id="ddeca-116">名称</span><span class="sxs-lookup"><span data-stu-id="ddeca-116">Name</span></span>       | <span data-ttu-id="ddeca-117">说明</span><span class="sxs-lookup"><span data-stu-id="ddeca-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ddeca-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddeca-118">Authorization</span></span>  | <span data-ttu-id="ddeca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddeca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddeca-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ddeca-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ddeca-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ddeca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddeca-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddeca-124">Request body</span></span>
<span data-ttu-id="ddeca-125">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddeca-125">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ddeca-126">响应</span><span class="sxs-lookup"><span data-stu-id="ddeca-126">Response</span></span>

<span data-ttu-id="ddeca-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ChartPoints](../resources/chartpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddeca-127">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddeca-128">示例</span><span class="sxs-lookup"><span data-stu-id="ddeca-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddeca-129">请求</span><span class="sxs-lookup"><span data-stu-id="ddeca-129">Request</span></span>
<span data-ttu-id="ddeca-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddeca-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="ddeca-131">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddeca-131">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ddeca-132">响应</span><span class="sxs-lookup"><span data-stu-id="ddeca-132">Response</span></span>
<span data-ttu-id="ddeca-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddeca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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