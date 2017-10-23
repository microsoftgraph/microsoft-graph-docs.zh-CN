# <a name="create-tablerow"></a><span data-ttu-id="6947e-101">创建 TableRow</span><span class="sxs-lookup"><span data-stu-id="6947e-101">Create TableRow</span></span>

<span data-ttu-id="6947e-102">使用此 API 创建新的 TableRow。</span><span class="sxs-lookup"><span data-stu-id="6947e-102">Use this API to create a new TableRow.</span></span>
## <a name="permissions"></a><span data-ttu-id="6947e-103">权限</span><span class="sxs-lookup"><span data-stu-id="6947e-103">Permissions</span></span>
<span data-ttu-id="6947e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6947e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6947e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="6947e-106">Permission type</span></span>      | <span data-ttu-id="6947e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6947e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6947e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6947e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6947e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6947e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6947e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6947e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6947e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6947e-111">Not supported.</span></span>    |
|<span data-ttu-id="6947e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6947e-112">Application</span></span> | <span data-ttu-id="6947e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6947e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6947e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6947e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows

```
## <a name="request-headers"></a><span data-ttu-id="6947e-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="6947e-115">Request headers</span></span>
| <span data-ttu-id="6947e-116">名称</span><span class="sxs-lookup"><span data-stu-id="6947e-116">Name</span></span>       | <span data-ttu-id="6947e-117">说明</span><span class="sxs-lookup"><span data-stu-id="6947e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6947e-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6947e-118">Authorization</span></span>  | <span data-ttu-id="6947e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6947e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6947e-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="6947e-121">Request body</span></span>
<span data-ttu-id="6947e-122">在请求正文中，提供 [TableRow](../resources/tablerow.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6947e-122">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6947e-123">响应</span><span class="sxs-lookup"><span data-stu-id="6947e-123">Response</span></span>

<span data-ttu-id="6947e-124">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6947e-124">If successful, this method returns `201 Created` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6947e-125">示例</span><span class="sxs-lookup"><span data-stu-id="6947e-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6947e-126">请求</span><span class="sxs-lookup"><span data-stu-id="6947e-126">Request</span></span>
<span data-ttu-id="6947e-127">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6947e-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablerow_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="6947e-128">在请求正文中，提供 [TableRow](../resources/tablerow.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6947e-128">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6947e-129">响应</span><span class="sxs-lookup"><span data-stu-id="6947e-129">Response</span></span>
<span data-ttu-id="6947e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6947e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->