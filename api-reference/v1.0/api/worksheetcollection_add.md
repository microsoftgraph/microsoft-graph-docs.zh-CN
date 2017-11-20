# <a name="worksheetcollection-add"></a><span data-ttu-id="0b705-101">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="0b705-101">WorksheetCollection: add</span></span>

<span data-ttu-id="0b705-p101">向工作簿添加新工作表。工作表将添加到现有工作表的末尾。如果您想要激活新添加的工作表，请对其调用 ".activate()。</span><span class="sxs-lookup"><span data-stu-id="0b705-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b705-105">权限</span><span class="sxs-lookup"><span data-stu-id="0b705-105">Permissions</span></span>
<span data-ttu-id="0b705-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0b705-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0b705-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b705-108">Permission type</span></span>      | <span data-ttu-id="0b705-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b705-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b705-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b705-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b705-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b705-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b705-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b705-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b705-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b705-113">Not supported.</span></span>    |
|<span data-ttu-id="0b705-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b705-114">Application</span></span> | <span data-ttu-id="0b705-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b705-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b705-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b705-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="0b705-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b705-117">Request headers</span></span>
| <span data-ttu-id="0b705-118">名称</span><span class="sxs-lookup"><span data-stu-id="0b705-118">Name</span></span>       | <span data-ttu-id="0b705-119">说明</span><span class="sxs-lookup"><span data-stu-id="0b705-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b705-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b705-120">Authorization</span></span>  | <span data-ttu-id="0b705-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b705-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b705-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b705-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b705-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0b705-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b705-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b705-126">Request body</span></span>
<span data-ttu-id="0b705-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0b705-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0b705-128">参数</span><span class="sxs-lookup"><span data-stu-id="0b705-128">Parameter</span></span>    | <span data-ttu-id="0b705-129">类型</span><span class="sxs-lookup"><span data-stu-id="0b705-129">Type</span></span>   |<span data-ttu-id="0b705-130">说明</span><span class="sxs-lookup"><span data-stu-id="0b705-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b705-131">name</span><span class="sxs-lookup"><span data-stu-id="0b705-131">name</span></span>|<span data-ttu-id="0b705-132">string</span><span class="sxs-lookup"><span data-stu-id="0b705-132">string</span></span>|<span data-ttu-id="0b705-p105">可选。要添加的工作表的名称。如果指定，名称应唯一。如果未指定，Excel 将确定新工作表的名称。</span><span class="sxs-lookup"><span data-stu-id="0b705-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="0b705-137">响应</span><span class="sxs-lookup"><span data-stu-id="0b705-137">Response</span></span>

<span data-ttu-id="0b705-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Worksheet](../resources/worksheet.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b705-138">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b705-139">示例</span><span class="sxs-lookup"><span data-stu-id="0b705-139">Example</span></span>
<span data-ttu-id="0b705-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0b705-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0b705-141">请求</span><span class="sxs-lookup"><span data-stu-id="0b705-141">Request</span></span>
<span data-ttu-id="0b705-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b705-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="0b705-143">响应</span><span class="sxs-lookup"><span data-stu-id="0b705-143">Response</span></span>
<span data-ttu-id="0b705-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b705-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->