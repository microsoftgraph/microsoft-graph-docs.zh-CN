# <a name="chart-setdata"></a><span data-ttu-id="8d6b1-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="8d6b1-101">Chart: setData</span></span>

<span data-ttu-id="8d6b1-102">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d6b1-103">权限</span><span class="sxs-lookup"><span data-stu-id="8d6b1-103">Permissions</span></span>
<span data-ttu-id="8d6b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8d6b1-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d6b1-106">Permission type</span></span>      | <span data-ttu-id="8d6b1-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d6b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d6b1-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d6b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8d6b1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d6b1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d6b1-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d6b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d6b1-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-111">Not supported.</span></span>    |
|<span data-ttu-id="8d6b1-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d6b1-112">Application</span></span> | <span data-ttu-id="8d6b1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d6b1-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d6b1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="8d6b1-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d6b1-115">Request headers</span></span>
| <span data-ttu-id="8d6b1-116">名称</span><span class="sxs-lookup"><span data-stu-id="8d6b1-116">Name</span></span>       | <span data-ttu-id="8d6b1-117">说明</span><span class="sxs-lookup"><span data-stu-id="8d6b1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d6b1-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d6b1-118">Authorization</span></span>  | <span data-ttu-id="8d6b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d6b1-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d6b1-121">Request body</span></span>
<span data-ttu-id="8d6b1-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d6b1-123">参数</span><span class="sxs-lookup"><span data-stu-id="8d6b1-123">Parameter</span></span>    | <span data-ttu-id="8d6b1-124">类型</span><span class="sxs-lookup"><span data-stu-id="8d6b1-124">Type</span></span>   |<span data-ttu-id="8d6b1-125">说明</span><span class="sxs-lookup"><span data-stu-id="8d6b1-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d6b1-126">sourceData</span><span class="sxs-lookup"><span data-stu-id="8d6b1-126">sourceData</span></span>|<span data-ttu-id="8d6b1-127">string</span><span class="sxs-lookup"><span data-stu-id="8d6b1-127">string</span></span>|<span data-ttu-id="8d6b1-128">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-128">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="8d6b1-129">seriesBy</span><span class="sxs-lookup"><span data-stu-id="8d6b1-129">seriesBy</span></span>|<span data-ttu-id="8d6b1-130">string</span><span class="sxs-lookup"><span data-stu-id="8d6b1-130">string</span></span>|<span data-ttu-id="8d6b1-p103">可选。指定列或行在图表上用作数据系列的方式。可以是下列值之一：自动（默认）、行、列。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-p103">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="8d6b1-135">响应</span><span class="sxs-lookup"><span data-stu-id="8d6b1-135">Response</span></span>

<span data-ttu-id="8d6b1-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d6b1-138">示例</span><span class="sxs-lookup"><span data-stu-id="8d6b1-138">Example</span></span>
<span data-ttu-id="8d6b1-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d6b1-140">请求</span><span class="sxs-lookup"><span data-stu-id="8d6b1-140">Request</span></span>
<span data-ttu-id="8d6b1-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="8d6b1-142">响应</span><span class="sxs-lookup"><span data-stu-id="8d6b1-142">Response</span></span>
<span data-ttu-id="8d6b1-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d6b1-143">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->