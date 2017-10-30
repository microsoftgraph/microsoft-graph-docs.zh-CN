# <a name="range-merge"></a><span data-ttu-id="fb055-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="fb055-101">Range: merge</span></span>

<span data-ttu-id="fb055-102">将范围单元格合并到工作表的一个区域中。</span><span class="sxs-lookup"><span data-stu-id="fb055-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb055-103">权限</span><span class="sxs-lookup"><span data-stu-id="fb055-103">Permissions</span></span>
<span data-ttu-id="fb055-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fb055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb055-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb055-106">Permission type</span></span>      | <span data-ttu-id="fb055-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb055-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb055-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb055-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fb055-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb055-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb055-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb055-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb055-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb055-111">Not supported.</span></span>    |
|<span data-ttu-id="fb055-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb055-112">Application</span></span> | <span data-ttu-id="fb055-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb055-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb055-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb055-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="fb055-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb055-115">Request headers</span></span>
| <span data-ttu-id="fb055-116">名称</span><span class="sxs-lookup"><span data-stu-id="fb055-116">Name</span></span>       | <span data-ttu-id="fb055-117">说明</span><span class="sxs-lookup"><span data-stu-id="fb055-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb055-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb055-118">Authorization</span></span>  | <span data-ttu-id="fb055-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb055-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb055-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb055-121">Request body</span></span>
<span data-ttu-id="fb055-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fb055-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fb055-123">参数</span><span class="sxs-lookup"><span data-stu-id="fb055-123">Parameter</span></span>    | <span data-ttu-id="fb055-124">类型</span><span class="sxs-lookup"><span data-stu-id="fb055-124">Type</span></span>   |<span data-ttu-id="fb055-125">说明</span><span class="sxs-lookup"><span data-stu-id="fb055-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb055-126">横向</span><span class="sxs-lookup"><span data-stu-id="fb055-126">across</span></span>|<span data-ttu-id="fb055-127">boolean</span><span class="sxs-lookup"><span data-stu-id="fb055-127">boolean</span></span>|<span data-ttu-id="fb055-p103">可选。如果为 True，则将指定区域中每一行的单元格合并为一个单独的合并单元格。默认值是 false。</span><span class="sxs-lookup"><span data-stu-id="fb055-p103">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="fb055-131">响应</span><span class="sxs-lookup"><span data-stu-id="fb055-131">Response</span></span>

<span data-ttu-id="fb055-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fb055-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb055-134">示例</span><span class="sxs-lookup"><span data-stu-id="fb055-134">Example</span></span>
<span data-ttu-id="fb055-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fb055-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fb055-136">请求</span><span class="sxs-lookup"><span data-stu-id="fb055-136">Request</span></span>
<span data-ttu-id="fb055-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb055-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="fb055-138">响应</span><span class="sxs-lookup"><span data-stu-id="fb055-138">Response</span></span>
<span data-ttu-id="fb055-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fb055-139">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->