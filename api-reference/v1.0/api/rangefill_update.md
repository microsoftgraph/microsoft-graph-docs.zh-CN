# <a name="update-rangefill"></a><span data-ttu-id="ac455-101">更新 rangefill</span><span class="sxs-lookup"><span data-stu-id="ac455-101">Update rangefill</span></span>

<span data-ttu-id="ac455-102">更新 rangefill 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ac455-102">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac455-103">权限</span><span class="sxs-lookup"><span data-stu-id="ac455-103">Permissions</span></span>
<span data-ttu-id="ac455-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ac455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac455-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac455-106">Permission type</span></span>      | <span data-ttu-id="ac455-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac455-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac455-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac455-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ac455-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac455-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ac455-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac455-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac455-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac455-111">Not supported.</span></span>    |
|<span data-ttu-id="ac455-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac455-112">Application</span></span> | <span data-ttu-id="ac455-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac455-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac455-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac455-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="ac455-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ac455-115">Optional request headers</span></span>
| <span data-ttu-id="ac455-116">名称</span><span class="sxs-lookup"><span data-stu-id="ac455-116">Name</span></span>       | <span data-ttu-id="ac455-117">说明</span><span class="sxs-lookup"><span data-stu-id="ac455-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac455-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac455-118">Authorization</span></span>  | <span data-ttu-id="ac455-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac455-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac455-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac455-121">Request body</span></span>
<span data-ttu-id="ac455-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ac455-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ac455-125">属性</span><span class="sxs-lookup"><span data-stu-id="ac455-125">Property</span></span>     | <span data-ttu-id="ac455-126">类型</span><span class="sxs-lookup"><span data-stu-id="ac455-126">Type</span></span>   |<span data-ttu-id="ac455-127">说明</span><span class="sxs-lookup"><span data-stu-id="ac455-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac455-128">color</span><span class="sxs-lookup"><span data-stu-id="ac455-128">color</span></span>|<span data-ttu-id="ac455-129">string</span><span class="sxs-lookup"><span data-stu-id="ac455-129">string</span></span>|<span data-ttu-id="ac455-130">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="ac455-130">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="ac455-131">响应</span><span class="sxs-lookup"><span data-stu-id="ac455-131">Response</span></span>

<span data-ttu-id="ac455-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Rangefill](../resources/rangefill.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac455-132">If successful, this method returns a `200 OK` response code and updated [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac455-133">示例</span><span class="sxs-lookup"><span data-stu-id="ac455-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac455-134">请求</span><span class="sxs-lookup"><span data-stu-id="ac455-134">Request</span></span>
<span data-ttu-id="ac455-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac455-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="ac455-136">响应</span><span class="sxs-lookup"><span data-stu-id="ac455-136">Response</span></span>
<span data-ttu-id="ac455-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac455-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->