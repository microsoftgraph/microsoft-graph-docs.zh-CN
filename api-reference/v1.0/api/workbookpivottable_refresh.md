# <a name="workbookpivottable-refresh"></a><span data-ttu-id="ca813-101">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="ca813-101">workbookPivotTable: refresh</span></span>

<span data-ttu-id="ca813-102">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="ca813-102">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="ca813-103">权限</span><span class="sxs-lookup"><span data-stu-id="ca813-103">Permissions</span></span>
<span data-ttu-id="ca813-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ca813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ca813-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca813-106">Permission type</span></span>      | <span data-ttu-id="ca813-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca813-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca813-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca813-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ca813-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca813-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca813-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca813-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca813-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca813-111">Not supported.</span></span>    |
|<span data-ttu-id="ca813-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca813-112">Application</span></span> | <span data-ttu-id="ca813-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca813-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca813-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca813-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="ca813-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca813-115">Request headers</span></span>
| <span data-ttu-id="ca813-116">名称</span><span class="sxs-lookup"><span data-stu-id="ca813-116">Name</span></span>       | <span data-ttu-id="ca813-117">说明</span><span class="sxs-lookup"><span data-stu-id="ca813-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca813-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca813-118">Authorization</span></span>  | <span data-ttu-id="ca813-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca813-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca813-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ca813-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ca813-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ca813-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca813-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca813-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="ca813-125">响应</span><span class="sxs-lookup"><span data-stu-id="ca813-125">Response</span></span>
<span data-ttu-id="ca813-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ca813-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca813-128">示例</span><span class="sxs-lookup"><span data-stu-id="ca813-128">Example</span></span>
<span data-ttu-id="ca813-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ca813-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ca813-130">请求</span><span class="sxs-lookup"><span data-stu-id="ca813-130">Request</span></span>
<span data-ttu-id="ca813-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca813-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="ca813-132">响应</span><span class="sxs-lookup"><span data-stu-id="ca813-132">Response</span></span>
<span data-ttu-id="ca813-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ca813-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
