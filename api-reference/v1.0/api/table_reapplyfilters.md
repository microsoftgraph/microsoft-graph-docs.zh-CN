# <a name="table-reapplyfilters"></a><span data-ttu-id="9307e-101">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="9307e-101">Table: reapplyFilters</span></span>

<span data-ttu-id="9307e-102">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="9307e-102">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9307e-103">权限</span><span class="sxs-lookup"><span data-stu-id="9307e-103">Permissions</span></span>
<span data-ttu-id="9307e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9307e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9307e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="9307e-106">Permission type</span></span>      | <span data-ttu-id="9307e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9307e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9307e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9307e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9307e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9307e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9307e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9307e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9307e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="9307e-111">Not supported.</span></span>    |
|<span data-ttu-id="9307e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="9307e-112">Application</span></span> | <span data-ttu-id="9307e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9307e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9307e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9307e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="9307e-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="9307e-115">Request headers</span></span>
| <span data-ttu-id="9307e-116">名称</span><span class="sxs-lookup"><span data-stu-id="9307e-116">Name</span></span>       | <span data-ttu-id="9307e-117">说明</span><span class="sxs-lookup"><span data-stu-id="9307e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9307e-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9307e-118">Authorization</span></span>  | <span data-ttu-id="9307e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9307e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9307e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9307e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9307e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9307e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9307e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9307e-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9307e-125">响应</span><span class="sxs-lookup"><span data-stu-id="9307e-125">Response</span></span>

<span data-ttu-id="9307e-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9307e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9307e-128">示例</span><span class="sxs-lookup"><span data-stu-id="9307e-128">Example</span></span>
<span data-ttu-id="9307e-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9307e-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9307e-130">请求</span><span class="sxs-lookup"><span data-stu-id="9307e-130">Request</span></span>
<span data-ttu-id="9307e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9307e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="9307e-132">响应</span><span class="sxs-lookup"><span data-stu-id="9307e-132">Response</span></span>
<span data-ttu-id="9307e-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9307e-133">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->