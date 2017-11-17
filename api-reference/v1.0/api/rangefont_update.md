# <a name="update-rangefont"></a><span data-ttu-id="8ff52-101">更新 rangefont</span><span class="sxs-lookup"><span data-stu-id="8ff52-101">Update rangefont</span></span>

<span data-ttu-id="8ff52-102">更新 rangefont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8ff52-102">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ff52-103">权限</span><span class="sxs-lookup"><span data-stu-id="8ff52-103">Permissions</span></span>
<span data-ttu-id="8ff52-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8ff52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ff52-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ff52-106">Permission type</span></span>      | <span data-ttu-id="8ff52-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ff52-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff52-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ff52-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff52-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff52-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ff52-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ff52-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff52-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ff52-111">Not supported.</span></span>    |
|<span data-ttu-id="8ff52-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ff52-112">Application</span></span> | <span data-ttu-id="8ff52-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ff52-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff52-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ff52-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="8ff52-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="8ff52-115">Optional request headers</span></span>
| <span data-ttu-id="8ff52-116">名称</span><span class="sxs-lookup"><span data-stu-id="8ff52-116">Name</span></span>       | <span data-ttu-id="8ff52-117">说明</span><span class="sxs-lookup"><span data-stu-id="8ff52-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8ff52-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ff52-118">Authorization</span></span>  | <span data-ttu-id="8ff52-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ff52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff52-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ff52-121">Request body</span></span>
<span data-ttu-id="8ff52-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8ff52-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8ff52-125">属性</span><span class="sxs-lookup"><span data-stu-id="8ff52-125">Property</span></span>     | <span data-ttu-id="8ff52-126">类型</span><span class="sxs-lookup"><span data-stu-id="8ff52-126">Type</span></span>   |<span data-ttu-id="8ff52-127">说明</span><span class="sxs-lookup"><span data-stu-id="8ff52-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ff52-128">bold</span><span class="sxs-lookup"><span data-stu-id="8ff52-128">bold</span></span>|<span data-ttu-id="8ff52-129">boolean</span><span class="sxs-lookup"><span data-stu-id="8ff52-129">boolean</span></span>|<span data-ttu-id="8ff52-130">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="8ff52-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="8ff52-131">color</span><span class="sxs-lookup"><span data-stu-id="8ff52-131">color</span></span>|<span data-ttu-id="8ff52-132">string</span><span class="sxs-lookup"><span data-stu-id="8ff52-132">string</span></span>|<span data-ttu-id="8ff52-p104">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="8ff52-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="8ff52-136">italic</span><span class="sxs-lookup"><span data-stu-id="8ff52-136">italic</span></span>|<span data-ttu-id="8ff52-137">boolean</span><span class="sxs-lookup"><span data-stu-id="8ff52-137">boolean</span></span>|<span data-ttu-id="8ff52-138">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="8ff52-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="8ff52-139">name</span><span class="sxs-lookup"><span data-stu-id="8ff52-139">name</span></span>|<span data-ttu-id="8ff52-140">string</span><span class="sxs-lookup"><span data-stu-id="8ff52-140">string</span></span>|<span data-ttu-id="8ff52-141">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="8ff52-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="8ff52-142">大小</span><span class="sxs-lookup"><span data-stu-id="8ff52-142">size</span></span>|<span data-ttu-id="8ff52-143">double</span><span class="sxs-lookup"><span data-stu-id="8ff52-143">double</span></span>|<span data-ttu-id="8ff52-144">字号</span><span class="sxs-lookup"><span data-stu-id="8ff52-144">Font size.</span></span>|
|<span data-ttu-id="8ff52-145">underline</span><span class="sxs-lookup"><span data-stu-id="8ff52-145">underline</span></span>|<span data-ttu-id="8ff52-146">string</span><span class="sxs-lookup"><span data-stu-id="8ff52-146">string</span></span>|<span data-ttu-id="8ff52-p105">应用于字体的下划线类型。可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="8ff52-p105">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="8ff52-149">响应</span><span class="sxs-lookup"><span data-stu-id="8ff52-149">Response</span></span>

<span data-ttu-id="8ff52-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeFont](../resources/rangefont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ff52-150">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ff52-151">示例</span><span class="sxs-lookup"><span data-stu-id="8ff52-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff52-152">请求</span><span class="sxs-lookup"><span data-stu-id="8ff52-152">Request</span></span>
<span data-ttu-id="8ff52-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ff52-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="8ff52-154">响应</span><span class="sxs-lookup"><span data-stu-id="8ff52-154">Response</span></span>
<span data-ttu-id="8ff52-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ff52-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->