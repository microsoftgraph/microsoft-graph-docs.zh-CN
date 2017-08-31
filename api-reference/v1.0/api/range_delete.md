# <a name="range-delete"></a><span data-ttu-id="79c7c-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="79c7c-101">Range: delete</span></span>

<span data-ttu-id="79c7c-102">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="79c7c-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="79c7c-103">权限</span><span class="sxs-lookup"><span data-stu-id="79c7c-103">Permissions</span></span>
<span data-ttu-id="79c7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="79c7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79c7c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="79c7c-106">Permission type</span></span>      | <span data-ttu-id="79c7c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79c7c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79c7c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79c7c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="79c7c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79c7c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79c7c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79c7c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79c7c-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="79c7c-111">Not supported.</span></span>    |
|<span data-ttu-id="79c7c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="79c7c-112">Application</span></span> | <span data-ttu-id="79c7c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="79c7c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79c7c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79c7c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="79c7c-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="79c7c-115">Request headers</span></span>
| <span data-ttu-id="79c7c-116">名称</span><span class="sxs-lookup"><span data-stu-id="79c7c-116">Name</span></span>       | <span data-ttu-id="79c7c-117">说明</span><span class="sxs-lookup"><span data-stu-id="79c7c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79c7c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="79c7c-118">Authorization</span></span>  | <span data-ttu-id="79c7c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79c7c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79c7c-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="79c7c-121">Request body</span></span>
<span data-ttu-id="79c7c-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="79c7c-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79c7c-123">参数</span><span class="sxs-lookup"><span data-stu-id="79c7c-123">Parameter</span></span>    | <span data-ttu-id="79c7c-124">类型</span><span class="sxs-lookup"><span data-stu-id="79c7c-124">Type</span></span>   |<span data-ttu-id="79c7c-125">说明</span><span class="sxs-lookup"><span data-stu-id="79c7c-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79c7c-126">Shift</span><span class="sxs-lookup"><span data-stu-id="79c7c-126">shift</span></span>|<span data-ttu-id="79c7c-127">string</span><span class="sxs-lookup"><span data-stu-id="79c7c-127">string</span></span>|<span data-ttu-id="79c7c-p103">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="79c7c-p103">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="79c7c-130">响应</span><span class="sxs-lookup"><span data-stu-id="79c7c-130">Response</span></span>

<span data-ttu-id="79c7c-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="79c7c-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79c7c-133">示例</span><span class="sxs-lookup"><span data-stu-id="79c7c-133">Example</span></span>
<span data-ttu-id="79c7c-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="79c7c-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79c7c-135">请求</span><span class="sxs-lookup"><span data-stu-id="79c7c-135">Request</span></span>
<span data-ttu-id="79c7c-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79c7c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="79c7c-137">响应</span><span class="sxs-lookup"><span data-stu-id="79c7c-137">Response</span></span>
<span data-ttu-id="79c7c-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="79c7c-138">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->