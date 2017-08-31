# <a name="create-table"></a><span data-ttu-id="636fe-101">创建表</span><span class="sxs-lookup"><span data-stu-id="636fe-101">Create Table</span></span>

<span data-ttu-id="636fe-102">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="636fe-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="636fe-103">权限</span><span class="sxs-lookup"><span data-stu-id="636fe-103">Permissions</span></span>
<span data-ttu-id="636fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="636fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="636fe-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="636fe-106">Permission type</span></span>      | <span data-ttu-id="636fe-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="636fe-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="636fe-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="636fe-108">Delegated (work or school account)</span></span> | <span data-ttu-id="636fe-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="636fe-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="636fe-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="636fe-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="636fe-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="636fe-111">Not supported.</span></span>    |
|<span data-ttu-id="636fe-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="636fe-112">Application</span></span> | <span data-ttu-id="636fe-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="636fe-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="636fe-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="636fe-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="636fe-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="636fe-115">Request headers</span></span>
| <span data-ttu-id="636fe-116">名称</span><span class="sxs-lookup"><span data-stu-id="636fe-116">Name</span></span>       | <span data-ttu-id="636fe-117">说明</span><span class="sxs-lookup"><span data-stu-id="636fe-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="636fe-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="636fe-118">Authorization</span></span>  | <span data-ttu-id="636fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="636fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="636fe-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="636fe-121">Request body</span></span>
<span data-ttu-id="636fe-122">在请求正文中，提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="636fe-122">In the request body, supply following parameters.</span></span> 

### <a name="request-parameters"></a><span data-ttu-id="636fe-123">请求参数</span><span class="sxs-lookup"><span data-stu-id="636fe-123">Request parameters</span></span>
| <span data-ttu-id="636fe-124">名称</span><span class="sxs-lookup"><span data-stu-id="636fe-124">Name</span></span>           | <span data-ttu-id="636fe-125">类型</span><span class="sxs-lookup"><span data-stu-id="636fe-125">Type</span></span>      |<span data-ttu-id="636fe-126">说明</span><span class="sxs-lookup"><span data-stu-id="636fe-126">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="636fe-127">Address</span><span class="sxs-lookup"><span data-stu-id="636fe-127">Address</span></span>  | <span data-ttu-id="636fe-128">string</span><span class="sxs-lookup"><span data-stu-id="636fe-128">string</span></span>| <span data-ttu-id="636fe-p103">区域地址。若要从 `worksheets/{id or name}/tables/add` 路径调用此 API，地址中无需有工作表名称前缀。不过，若要从 `workbook/tables/add` 路径调用此 API，请提供需要在其中创建表的工作表名称（例如：`sheet1!A1:D4`）</span><span class="sxs-lookup"><span data-stu-id="636fe-p103">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="636fe-132">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="636fe-132">hasHeaders</span></span>  | <span data-ttu-id="636fe-133">布尔</span><span class="sxs-lookup"><span data-stu-id="636fe-133">boolean</span></span>|<span data-ttu-id="636fe-p104">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="636fe-p104">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="636fe-137">响应</span><span class="sxs-lookup"><span data-stu-id="636fe-137">Response</span></span>

<span data-ttu-id="636fe-138">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="636fe-138">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="636fe-139">示例</span><span class="sxs-lookup"><span data-stu-id="636fe-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="636fe-140">请求</span><span class="sxs-lookup"><span data-stu-id="636fe-140">Request</span></span>
<span data-ttu-id="636fe-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="636fe-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="636fe-142">响应</span><span class="sxs-lookup"><span data-stu-id="636fe-142">Response</span></span>
<span data-ttu-id="636fe-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="636fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
