# <a name="update-chartfont"></a><span data-ttu-id="173ce-101">更新 chartfont</span><span class="sxs-lookup"><span data-stu-id="173ce-101">Update chartfont</span></span>

<span data-ttu-id="173ce-102">更新 chartfont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="173ce-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="173ce-103">权限</span><span class="sxs-lookup"><span data-stu-id="173ce-103">Permissions</span></span>
<span data-ttu-id="173ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="173ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="173ce-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="173ce-106">Permission type</span></span>      | <span data-ttu-id="173ce-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="173ce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="173ce-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="173ce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="173ce-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="173ce-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="173ce-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="173ce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="173ce-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="173ce-111">Not supported.</span></span>    |
|<span data-ttu-id="173ce-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="173ce-112">Application</span></span> | <span data-ttu-id="173ce-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="173ce-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="173ce-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="173ce-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="173ce-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="173ce-115">Optional request headers</span></span>
| <span data-ttu-id="173ce-116">名称</span><span class="sxs-lookup"><span data-stu-id="173ce-116">Name</span></span>       | <span data-ttu-id="173ce-117">说明</span><span class="sxs-lookup"><span data-stu-id="173ce-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="173ce-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="173ce-118">Authorization</span></span>  | <span data-ttu-id="173ce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="173ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="173ce-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="173ce-121">Request body</span></span>
<span data-ttu-id="173ce-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="173ce-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="173ce-125">属性</span><span class="sxs-lookup"><span data-stu-id="173ce-125">Property</span></span>     | <span data-ttu-id="173ce-126">类型</span><span class="sxs-lookup"><span data-stu-id="173ce-126">Type</span></span>   |<span data-ttu-id="173ce-127">说明</span><span class="sxs-lookup"><span data-stu-id="173ce-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="173ce-128">bold</span><span class="sxs-lookup"><span data-stu-id="173ce-128">bold</span></span>|<span data-ttu-id="173ce-129">boolean</span><span class="sxs-lookup"><span data-stu-id="173ce-129">boolean</span></span>|<span data-ttu-id="173ce-130">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="173ce-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="173ce-131">color</span><span class="sxs-lookup"><span data-stu-id="173ce-131">color</span></span>|<span data-ttu-id="173ce-132">string</span><span class="sxs-lookup"><span data-stu-id="173ce-132">string</span></span>|<span data-ttu-id="173ce-p104">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="173ce-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="173ce-136">italic</span><span class="sxs-lookup"><span data-stu-id="173ce-136">italic</span></span>|<span data-ttu-id="173ce-137">boolean</span><span class="sxs-lookup"><span data-stu-id="173ce-137">boolean</span></span>|<span data-ttu-id="173ce-138">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="173ce-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="173ce-139">name</span><span class="sxs-lookup"><span data-stu-id="173ce-139">name</span></span>|<span data-ttu-id="173ce-140">string</span><span class="sxs-lookup"><span data-stu-id="173ce-140">string</span></span>|<span data-ttu-id="173ce-141">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="173ce-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="173ce-142">大小</span><span class="sxs-lookup"><span data-stu-id="173ce-142">size</span></span>|<span data-ttu-id="173ce-143">double</span><span class="sxs-lookup"><span data-stu-id="173ce-143">double</span></span>|<span data-ttu-id="173ce-144">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="173ce-144">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="173ce-145">underline</span><span class="sxs-lookup"><span data-stu-id="173ce-145">underline</span></span>|<span data-ttu-id="173ce-146">string</span><span class="sxs-lookup"><span data-stu-id="173ce-146">string</span></span>|<span data-ttu-id="173ce-p105">应用于字体的下划线类型。可能的值是：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="173ce-p105">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="173ce-149">响应</span><span class="sxs-lookup"><span data-stu-id="173ce-149">Response</span></span>

<span data-ttu-id="173ce-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartFont](../resources/chartfont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="173ce-150">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="173ce-151">示例</span><span class="sxs-lookup"><span data-stu-id="173ce-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="173ce-152">请求</span><span class="sxs-lookup"><span data-stu-id="173ce-152">Request</span></span>
<span data-ttu-id="173ce-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="173ce-153">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="173ce-154">响应</span><span class="sxs-lookup"><span data-stu-id="173ce-154">Response</span></span>
<span data-ttu-id="173ce-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="173ce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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