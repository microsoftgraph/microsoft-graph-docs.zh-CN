# <a name="refresh-session"></a><span data-ttu-id="9cc73-101">刷新会话</span><span class="sxs-lookup"><span data-stu-id="9cc73-101">Refresh Session</span></span>

<span data-ttu-id="9cc73-102">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="9cc73-102">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9cc73-103">权限</span><span class="sxs-lookup"><span data-stu-id="9cc73-103">Permissions</span></span>
<span data-ttu-id="9cc73-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9cc73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9cc73-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc73-106">Permission type</span></span>      | <span data-ttu-id="9cc73-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cc73-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc73-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc73-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9cc73-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cc73-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9cc73-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc73-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc73-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc73-111">Not supported.</span></span>    |
|<span data-ttu-id="9cc73-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cc73-112">Application</span></span> | <span data-ttu-id="9cc73-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc73-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc73-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc73-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="9cc73-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cc73-115">Request headers</span></span>
| <span data-ttu-id="9cc73-116">名称</span><span class="sxs-lookup"><span data-stu-id="9cc73-116">Name</span></span>       | <span data-ttu-id="9cc73-117">说明</span><span class="sxs-lookup"><span data-stu-id="9cc73-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9cc73-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc73-118">Authorization</span></span>  | <span data-ttu-id="9cc73-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cc73-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cc73-121">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="9cc73-121">workbook-session-id</span></span> | <span data-ttu-id="9cc73-122">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="9cc73-122">Workbook session Id to be refreshd</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cc73-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc73-123">Request body</span></span>
<span data-ttu-id="9cc73-124">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cc73-124">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="9cc73-125">响应</span><span class="sxs-lookup"><span data-stu-id="9cc73-125">Response</span></span>

<span data-ttu-id="9cc73-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9cc73-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9cc73-127">示例</span><span class="sxs-lookup"><span data-stu-id="9cc73-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cc73-128">请求</span><span class="sxs-lookup"><span data-stu-id="9cc73-128">Request</span></span>
<span data-ttu-id="9cc73-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cc73-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="9cc73-130">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="9cc73-130">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="9cc73-131">响应</span><span class="sxs-lookup"><span data-stu-id="9cc73-131">Response</span></span>
<span data-ttu-id="9cc73-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9cc73-132">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```