# <a name="tablesort-clear"></a><span data-ttu-id="181f6-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="181f6-101">TableSort: clear</span></span>

<span data-ttu-id="181f6-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="181f6-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="181f6-104">权限</span><span class="sxs-lookup"><span data-stu-id="181f6-104">Permissions</span></span>
<span data-ttu-id="181f6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="181f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="181f6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="181f6-107">Permission type</span></span>      | <span data-ttu-id="181f6-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="181f6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181f6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="181f6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="181f6-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181f6-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="181f6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="181f6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181f6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="181f6-112">Not supported.</span></span>    |
|<span data-ttu-id="181f6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="181f6-113">Application</span></span> | <span data-ttu-id="181f6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="181f6-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="181f6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="181f6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="181f6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="181f6-116">Request headers</span></span>
| <span data-ttu-id="181f6-117">名称</span><span class="sxs-lookup"><span data-stu-id="181f6-117">Name</span></span>       | <span data-ttu-id="181f6-118">说明</span><span class="sxs-lookup"><span data-stu-id="181f6-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="181f6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="181f6-119">Authorization</span></span>  | <span data-ttu-id="181f6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="181f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="181f6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="181f6-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="181f6-123">响应</span><span class="sxs-lookup"><span data-stu-id="181f6-123">Response</span></span>

<span data-ttu-id="181f6-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="181f6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181f6-126">示例</span><span class="sxs-lookup"><span data-stu-id="181f6-126">Example</span></span>
<span data-ttu-id="181f6-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="181f6-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="181f6-128">请求</span><span class="sxs-lookup"><span data-stu-id="181f6-128">Request</span></span>
<span data-ttu-id="181f6-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="181f6-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="181f6-130">响应</span><span class="sxs-lookup"><span data-stu-id="181f6-130">Response</span></span>
<span data-ttu-id="181f6-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="181f6-131">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->