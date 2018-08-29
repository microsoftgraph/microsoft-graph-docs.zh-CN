# <a name="tablesort-clear"></a><span data-ttu-id="c98aa-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="c98aa-101">TableSort: clear</span></span>

<span data-ttu-id="c98aa-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="c98aa-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="c98aa-104">权限</span><span class="sxs-lookup"><span data-stu-id="c98aa-104">Permissions</span></span>
<span data-ttu-id="c98aa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c98aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c98aa-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c98aa-107">Permission type</span></span>      | <span data-ttu-id="c98aa-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c98aa-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c98aa-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c98aa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c98aa-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c98aa-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c98aa-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c98aa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c98aa-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c98aa-112">Not supported.</span></span>    |
|<span data-ttu-id="c98aa-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c98aa-113">Application</span></span> | <span data-ttu-id="c98aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c98aa-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c98aa-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c98aa-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="c98aa-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c98aa-116">Request headers</span></span>
| <span data-ttu-id="c98aa-117">名称</span><span class="sxs-lookup"><span data-stu-id="c98aa-117">Name</span></span>       | <span data-ttu-id="c98aa-118">说明</span><span class="sxs-lookup"><span data-stu-id="c98aa-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c98aa-119">授权</span><span class="sxs-lookup"><span data-stu-id="c98aa-119">Authorization</span></span>  | <span data-ttu-id="c98aa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c98aa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c98aa-122">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c98aa-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="c98aa-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c98aa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c98aa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c98aa-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c98aa-126">响应</span><span class="sxs-lookup"><span data-stu-id="c98aa-126">Response</span></span>

<span data-ttu-id="c98aa-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c98aa-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c98aa-129">示例</span><span class="sxs-lookup"><span data-stu-id="c98aa-129">Example</span></span>
<span data-ttu-id="c98aa-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c98aa-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c98aa-131">请求</span><span class="sxs-lookup"><span data-stu-id="c98aa-131">Request</span></span>
<span data-ttu-id="c98aa-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c98aa-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="c98aa-133">响应</span><span class="sxs-lookup"><span data-stu-id="c98aa-133">Response</span></span>
<span data-ttu-id="c98aa-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c98aa-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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