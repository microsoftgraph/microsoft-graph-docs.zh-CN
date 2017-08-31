# <a name="update-rangeformat"></a><span data-ttu-id="6a1ad-101">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="6a1ad-101">Update rangeformat</span></span>

<span data-ttu-id="6a1ad-102">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a1ad-103">权限</span><span class="sxs-lookup"><span data-stu-id="6a1ad-103">Permissions</span></span>
<span data-ttu-id="6a1ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a1ad-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a1ad-106">Permission type</span></span>      | <span data-ttu-id="6a1ad-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a1ad-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a1ad-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a1ad-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6a1ad-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a1ad-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a1ad-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a1ad-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a1ad-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-111">Not supported.</span></span>    |
|<span data-ttu-id="6a1ad-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a1ad-112">Application</span></span> | <span data-ttu-id="6a1ad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a1ad-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a1ad-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(<address>)/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="6a1ad-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="6a1ad-115">Optional request headers</span></span>
| <span data-ttu-id="6a1ad-116">名称</span><span class="sxs-lookup"><span data-stu-id="6a1ad-116">Name</span></span>       | <span data-ttu-id="6a1ad-117">说明</span><span class="sxs-lookup"><span data-stu-id="6a1ad-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6a1ad-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a1ad-118">Authorization</span></span>  | <span data-ttu-id="6a1ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a1ad-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a1ad-121">Request body</span></span>
<span data-ttu-id="6a1ad-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6a1ad-125">属性</span><span class="sxs-lookup"><span data-stu-id="6a1ad-125">Property</span></span>     | <span data-ttu-id="6a1ad-126">类型</span><span class="sxs-lookup"><span data-stu-id="6a1ad-126">Type</span></span>   |<span data-ttu-id="6a1ad-127">说明</span><span class="sxs-lookup"><span data-stu-id="6a1ad-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a1ad-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="6a1ad-128">columnWidth</span></span>|<span data-ttu-id="6a1ad-129">double</span><span class="sxs-lookup"><span data-stu-id="6a1ad-129">double</span></span>|<span data-ttu-id="6a1ad-p104">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="6a1ad-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="6a1ad-132">horizontalAlignment</span></span>|<span data-ttu-id="6a1ad-133">string</span><span class="sxs-lookup"><span data-stu-id="6a1ad-133">string</span></span>|<span data-ttu-id="6a1ad-p105">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="6a1ad-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="6a1ad-136">rowHeight</span></span>|<span data-ttu-id="6a1ad-137">double</span><span class="sxs-lookup"><span data-stu-id="6a1ad-137">double</span></span>|<span data-ttu-id="6a1ad-p106">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="6a1ad-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="6a1ad-140">verticalAlignment</span></span>|<span data-ttu-id="6a1ad-141">string</span><span class="sxs-lookup"><span data-stu-id="6a1ad-141">string</span></span>|<span data-ttu-id="6a1ad-p107">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="6a1ad-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="6a1ad-144">wrapText</span></span>|<span data-ttu-id="6a1ad-145">boolean</span><span class="sxs-lookup"><span data-stu-id="6a1ad-145">boolean</span></span>|<span data-ttu-id="6a1ad-p108">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="6a1ad-148">响应</span><span class="sxs-lookup"><span data-stu-id="6a1ad-148">Response</span></span>

<span data-ttu-id="6a1ad-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeFormat](../resources/rangeformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a1ad-150">示例</span><span class="sxs-lookup"><span data-stu-id="6a1ad-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a1ad-151">请求</span><span class="sxs-lookup"><span data-stu-id="6a1ad-151">Request</span></span>
<span data-ttu-id="6a1ad-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```
##### <a name="response"></a><span data-ttu-id="6a1ad-153">响应</span><span class="sxs-lookup"><span data-stu-id="6a1ad-153">Response</span></span>
<span data-ttu-id="6a1ad-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a1ad-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->