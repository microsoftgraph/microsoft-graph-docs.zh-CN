# <a name="update-rangeborder"></a><span data-ttu-id="b9f66-101">更新 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="b9f66-101">Update rangeborder</span></span>

<span data-ttu-id="b9f66-102">更新 rangeborder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9f66-102">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9f66-103">权限</span><span class="sxs-lookup"><span data-stu-id="b9f66-103">Permissions</span></span>
<span data-ttu-id="b9f66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b9f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9f66-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9f66-106">Permission type</span></span>      | <span data-ttu-id="b9f66-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9f66-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9f66-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9f66-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9f66-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f66-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9f66-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9f66-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f66-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9f66-111">Not supported.</span></span>    |
|<span data-ttu-id="b9f66-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9f66-112">Application</span></span> | <span data-ttu-id="b9f66-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9f66-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9f66-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9f66-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="b9f66-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b9f66-115">Optional request headers</span></span>
| <span data-ttu-id="b9f66-116">名称</span><span class="sxs-lookup"><span data-stu-id="b9f66-116">Name</span></span>       | <span data-ttu-id="b9f66-117">说明</span><span class="sxs-lookup"><span data-stu-id="b9f66-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b9f66-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f66-118">Authorization</span></span>  | <span data-ttu-id="b9f66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9f66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9f66-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9f66-121">Request body</span></span>
<span data-ttu-id="b9f66-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9f66-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9f66-125">属性</span><span class="sxs-lookup"><span data-stu-id="b9f66-125">Property</span></span>     | <span data-ttu-id="b9f66-126">类型</span><span class="sxs-lookup"><span data-stu-id="b9f66-126">Type</span></span>   |<span data-ttu-id="b9f66-127">说明</span><span class="sxs-lookup"><span data-stu-id="b9f66-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9f66-128">color</span><span class="sxs-lookup"><span data-stu-id="b9f66-128">color</span></span>|<span data-ttu-id="b9f66-129">string</span><span class="sxs-lookup"><span data-stu-id="b9f66-129">string</span></span>|<span data-ttu-id="b9f66-130">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="b9f66-130">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="b9f66-131">style</span><span class="sxs-lookup"><span data-stu-id="b9f66-131">style</span></span>|<span data-ttu-id="b9f66-132">string</span><span class="sxs-lookup"><span data-stu-id="b9f66-132">string</span></span>|<span data-ttu-id="b9f66-p104">线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="b9f66-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="b9f66-135">weight</span><span class="sxs-lookup"><span data-stu-id="b9f66-135">weight</span></span>|<span data-ttu-id="b9f66-136">string</span><span class="sxs-lookup"><span data-stu-id="b9f66-136">string</span></span>|<span data-ttu-id="b9f66-p105">指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="b9f66-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="b9f66-139">响应</span><span class="sxs-lookup"><span data-stu-id="b9f66-139">Response</span></span>

<span data-ttu-id="b9f66-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeBorder](../resources/rangeborder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9f66-140">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9f66-141">示例</span><span class="sxs-lookup"><span data-stu-id="b9f66-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9f66-142">请求</span><span class="sxs-lookup"><span data-stu-id="b9f66-142">Request</span></span>
<span data-ttu-id="b9f66-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9f66-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="b9f66-144">响应</span><span class="sxs-lookup"><span data-stu-id="b9f66-144">Response</span></span>
<span data-ttu-id="b9f66-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9f66-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->