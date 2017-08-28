# <a name="update-formatprotection"></a><span data-ttu-id="b4d1f-101">更新 formatProtection</span><span class="sxs-lookup"><span data-stu-id="b4d1f-101">Update formatprotection</span></span>

<span data-ttu-id="b4d1f-102">更新 formatprotection 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-102">Update the properties of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4d1f-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4d1f-103">Prerequisites</span></span>
<span data-ttu-id="b4d1f-104">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="b4d1f-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="b4d1f-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4d1f-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="b4d1f-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4d1f-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="b4d1f-107">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b4d1f-107">Optional request headers</span></span>
| <span data-ttu-id="b4d1f-108">名称</span><span class="sxs-lookup"><span data-stu-id="b4d1f-108">Name</span></span>       | <span data-ttu-id="b4d1f-109">说明</span><span class="sxs-lookup"><span data-stu-id="b4d1f-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4d1f-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4d1f-110">Authorization</span></span>  | <span data-ttu-id="b4d1f-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4d1f-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4d1f-113">Request body</span></span>
<span data-ttu-id="b4d1f-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4d1f-117">属性</span><span class="sxs-lookup"><span data-stu-id="b4d1f-117">Property</span></span>     | <span data-ttu-id="b4d1f-118">类型</span><span class="sxs-lookup"><span data-stu-id="b4d1f-118">Type</span></span>   |<span data-ttu-id="b4d1f-119">说明</span><span class="sxs-lookup"><span data-stu-id="b4d1f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4d1f-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="b4d1f-120">formulaHidden</span></span>|<span data-ttu-id="b4d1f-121">boolean</span><span class="sxs-lookup"><span data-stu-id="b4d1f-121">boolean</span></span>|<span data-ttu-id="b4d1f-p103">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p103">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="b4d1f-124">已锁定</span><span class="sxs-lookup"><span data-stu-id="b4d1f-124">locked</span></span>|<span data-ttu-id="b4d1f-125">boolean</span><span class="sxs-lookup"><span data-stu-id="b4d1f-125">boolean</span></span>|<span data-ttu-id="b4d1f-p104">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p104">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="b4d1f-128">响应</span><span class="sxs-lookup"><span data-stu-id="b4d1f-128">Response</span></span>

<span data-ttu-id="b4d1f-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-129">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4d1f-130">示例</span><span class="sxs-lookup"><span data-stu-id="b4d1f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4d1f-131">请求</span><span class="sxs-lookup"><span data-stu-id="b4d1f-131">Request</span></span>
<span data-ttu-id="b4d1f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="b4d1f-133">响应</span><span class="sxs-lookup"><span data-stu-id="b4d1f-133">Response</span></span>
<span data-ttu-id="b4d1f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4d1f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->