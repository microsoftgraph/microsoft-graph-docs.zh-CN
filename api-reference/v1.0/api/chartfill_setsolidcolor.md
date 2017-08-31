# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="089f0-101">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="089f0-101">ChartFill: setSolidColor</span></span>

<span data-ttu-id="089f0-102">将图表元素的填充格式设置为统一颜色。</span><span class="sxs-lookup"><span data-stu-id="089f0-102">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="089f0-103">权限</span><span class="sxs-lookup"><span data-stu-id="089f0-103">Permissions</span></span>
<span data-ttu-id="089f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="089f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="089f0-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="089f0-106">Permission type</span></span>      | <span data-ttu-id="089f0-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="089f0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="089f0-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="089f0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="089f0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="089f0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="089f0-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="089f0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="089f0-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="089f0-111">Not supported.</span></span>    |
|<span data-ttu-id="089f0-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="089f0-112">Application</span></span> | <span data-ttu-id="089f0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="089f0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="089f0-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="089f0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="089f0-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="089f0-115">Request headers</span></span>
| <span data-ttu-id="089f0-116">名称</span><span class="sxs-lookup"><span data-stu-id="089f0-116">Name</span></span>       | <span data-ttu-id="089f0-117">说明</span><span class="sxs-lookup"><span data-stu-id="089f0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="089f0-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="089f0-118">Authorization</span></span>  | <span data-ttu-id="089f0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="089f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="089f0-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="089f0-121">Request body</span></span>
<span data-ttu-id="089f0-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="089f0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="089f0-123">参数</span><span class="sxs-lookup"><span data-stu-id="089f0-123">Parameter</span></span>    | <span data-ttu-id="089f0-124">类型</span><span class="sxs-lookup"><span data-stu-id="089f0-124">Type</span></span>   |<span data-ttu-id="089f0-125">说明</span><span class="sxs-lookup"><span data-stu-id="089f0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="089f0-126">color</span><span class="sxs-lookup"><span data-stu-id="089f0-126">color</span></span>|<span data-ttu-id="089f0-127">string</span><span class="sxs-lookup"><span data-stu-id="089f0-127">string</span></span>|<span data-ttu-id="089f0-128">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="089f0-128">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="089f0-129">响应</span><span class="sxs-lookup"><span data-stu-id="089f0-129">Response</span></span>

<span data-ttu-id="089f0-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="089f0-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="089f0-132">示例</span><span class="sxs-lookup"><span data-stu-id="089f0-132">Example</span></span>
<span data-ttu-id="089f0-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="089f0-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="089f0-134">请求</span><span class="sxs-lookup"><span data-stu-id="089f0-134">Request</span></span>
<span data-ttu-id="089f0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="089f0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="089f0-136">响应</span><span class="sxs-lookup"><span data-stu-id="089f0-136">Response</span></span>
<span data-ttu-id="089f0-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="089f0-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->