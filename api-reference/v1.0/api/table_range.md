# <a name="table-range"></a><span data-ttu-id="5fc5f-101">Table:Range</span><span class="sxs-lookup"><span data-stu-id="5fc5f-101">Table: Range</span></span>

<span data-ttu-id="5fc5f-102">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-102">Gets the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5fc5f-103">权限</span><span class="sxs-lookup"><span data-stu-id="5fc5f-103">Permissions</span></span>
<span data-ttu-id="5fc5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5fc5f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fc5f-106">Permission type</span></span>      | <span data-ttu-id="5fc5f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5fc5f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fc5f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fc5f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5fc5f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5fc5f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5fc5f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fc5f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fc5f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-111">Not supported.</span></span>    |
|<span data-ttu-id="5fc5f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fc5f-112">Application</span></span> | <span data-ttu-id="5fc5f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fc5f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fc5f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="5fc5f-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fc5f-115">Request headers</span></span>
| <span data-ttu-id="5fc5f-116">名称</span><span class="sxs-lookup"><span data-stu-id="5fc5f-116">Name</span></span>       | <span data-ttu-id="5fc5f-117">说明</span><span class="sxs-lookup"><span data-stu-id="5fc5f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5fc5f-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fc5f-118">Authorization</span></span>  | <span data-ttu-id="5fc5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fc5f-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fc5f-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5fc5f-122">响应</span><span class="sxs-lookup"><span data-stu-id="5fc5f-122">Response</span></span>

<span data-ttu-id="5fc5f-123">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-123">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fc5f-124">示例</span><span class="sxs-lookup"><span data-stu-id="5fc5f-124">Example</span></span>
<span data-ttu-id="5fc5f-125">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5fc5f-126">请求</span><span class="sxs-lookup"><span data-stu-id="5fc5f-126">Request</span></span>
<span data-ttu-id="5fc5f-127">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/Range
```

##### <a name="response"></a><span data-ttu-id="5fc5f-128">响应</span><span class="sxs-lookup"><span data-stu-id="5fc5f-128">Response</span></span>
<span data-ttu-id="5fc5f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fc5f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->