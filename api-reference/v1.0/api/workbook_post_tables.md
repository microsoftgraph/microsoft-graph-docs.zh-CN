# <a name="create-table"></a><span data-ttu-id="6c5db-101">创建表</span><span class="sxs-lookup"><span data-stu-id="6c5db-101">Create Table</span></span>

<span data-ttu-id="6c5db-102">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="6c5db-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c5db-103">权限</span><span class="sxs-lookup"><span data-stu-id="6c5db-103">Permissions</span></span>
<span data-ttu-id="6c5db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6c5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c5db-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c5db-106">Permission type</span></span>      | <span data-ttu-id="6c5db-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c5db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c5db-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c5db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6c5db-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c5db-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c5db-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c5db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c5db-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c5db-111">Not supported.</span></span>    |
|<span data-ttu-id="6c5db-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c5db-112">Application</span></span> | <span data-ttu-id="6c5db-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c5db-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c5db-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c5db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="6c5db-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c5db-115">Request headers</span></span>
| <span data-ttu-id="6c5db-116">名称</span><span class="sxs-lookup"><span data-stu-id="6c5db-116">Name</span></span>       | <span data-ttu-id="6c5db-117">说明</span><span class="sxs-lookup"><span data-stu-id="6c5db-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6c5db-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c5db-118">Authorization</span></span>  | <span data-ttu-id="6c5db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c5db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c5db-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c5db-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c5db-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6c5db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c5db-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c5db-124">Request body</span></span>
<span data-ttu-id="6c5db-125">在请求正文中，提供 [Table](../resources/table.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c5db-125">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6c5db-126">响应</span><span class="sxs-lookup"><span data-stu-id="6c5db-126">Response</span></span>

<span data-ttu-id="6c5db-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c5db-127">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c5db-128">示例</span><span class="sxs-lookup"><span data-stu-id="6c5db-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c5db-129">请求</span><span class="sxs-lookup"><span data-stu-id="6c5db-129">Request</span></span>
<span data-ttu-id="6c5db-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c5db-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "id": 99,
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
<span data-ttu-id="6c5db-131">在请求正文中，提供 [Table](../resources/table.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c5db-131">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6c5db-132">响应</span><span class="sxs-lookup"><span data-stu-id="6c5db-132">Response</span></span>
<span data-ttu-id="6c5db-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c5db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
