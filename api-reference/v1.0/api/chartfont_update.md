# <a name="update-chartfont"></a><span data-ttu-id="d362e-101">更新 chartfont</span><span class="sxs-lookup"><span data-stu-id="d362e-101">Update chartfont</span></span>

<span data-ttu-id="d362e-102">更新 chartfont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d362e-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d362e-103">权限</span><span class="sxs-lookup"><span data-stu-id="d362e-103">Permissions</span></span>
<span data-ttu-id="d362e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d362e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d362e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d362e-106">Permission type</span></span>      | <span data-ttu-id="d362e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d362e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d362e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d362e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d362e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d362e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d362e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d362e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d362e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d362e-111">Not supported.</span></span>    |
|<span data-ttu-id="d362e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d362e-112">Application</span></span> | <span data-ttu-id="d362e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d362e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d362e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d362e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="d362e-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d362e-115">Optional request headers</span></span>
| <span data-ttu-id="d362e-116">名称</span><span class="sxs-lookup"><span data-stu-id="d362e-116">Name</span></span>       | <span data-ttu-id="d362e-117">说明</span><span class="sxs-lookup"><span data-stu-id="d362e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d362e-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d362e-118">Authorization</span></span>  | <span data-ttu-id="d362e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d362e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d362e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d362e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="d362e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d362e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d362e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d362e-124">Request body</span></span>
<span data-ttu-id="d362e-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d362e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d362e-128">属性</span><span class="sxs-lookup"><span data-stu-id="d362e-128">Property</span></span>     | <span data-ttu-id="d362e-129">类型</span><span class="sxs-lookup"><span data-stu-id="d362e-129">Type</span></span>   |<span data-ttu-id="d362e-130">说明</span><span class="sxs-lookup"><span data-stu-id="d362e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d362e-131">bold</span><span class="sxs-lookup"><span data-stu-id="d362e-131">bold</span></span>|<span data-ttu-id="d362e-132">布尔</span><span class="sxs-lookup"><span data-stu-id="d362e-132">boolean</span></span>|<span data-ttu-id="d362e-133">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="d362e-133">Represents the bold status of font.</span></span>|
|<span data-ttu-id="d362e-134">color</span><span class="sxs-lookup"><span data-stu-id="d362e-134">color</span></span>|<span data-ttu-id="d362e-135">string</span><span class="sxs-lookup"><span data-stu-id="d362e-135">string</span></span>|<span data-ttu-id="d362e-p105">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="d362e-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="d362e-139">italic</span><span class="sxs-lookup"><span data-stu-id="d362e-139">italic</span></span>|<span data-ttu-id="d362e-140">布尔</span><span class="sxs-lookup"><span data-stu-id="d362e-140">boolean</span></span>|<span data-ttu-id="d362e-141">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="d362e-141">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="d362e-142">name</span><span class="sxs-lookup"><span data-stu-id="d362e-142">name</span></span>|<span data-ttu-id="d362e-143">string</span><span class="sxs-lookup"><span data-stu-id="d362e-143">string</span></span>|<span data-ttu-id="d362e-144">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="d362e-144">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="d362e-145">大小</span><span class="sxs-lookup"><span data-stu-id="d362e-145">size</span></span>|<span data-ttu-id="d362e-146">double</span><span class="sxs-lookup"><span data-stu-id="d362e-146">double</span></span>|<span data-ttu-id="d362e-147">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="d362e-147">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="d362e-148">underline</span><span class="sxs-lookup"><span data-stu-id="d362e-148">underline</span></span>|<span data-ttu-id="d362e-149">string</span><span class="sxs-lookup"><span data-stu-id="d362e-149">string</span></span>|<span data-ttu-id="d362e-p106">应用于字体的下划线类型。可能的值是：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="d362e-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="d362e-152">响应</span><span class="sxs-lookup"><span data-stu-id="d362e-152">Response</span></span>

<span data-ttu-id="d362e-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartFont](../resources/chartfont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d362e-153">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d362e-154">示例</span><span class="sxs-lookup"><span data-stu-id="d362e-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d362e-155">请求</span><span class="sxs-lookup"><span data-stu-id="d362e-155">Request</span></span>
<span data-ttu-id="d362e-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d362e-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="d362e-157">响应</span><span class="sxs-lookup"><span data-stu-id="d362e-157">Response</span></span>
<span data-ttu-id="d362e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d362e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->