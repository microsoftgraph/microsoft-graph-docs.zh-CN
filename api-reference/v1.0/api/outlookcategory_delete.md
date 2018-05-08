# <a name="delete-outlook-category"></a><span data-ttu-id="28b41-101">删除 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="28b41-101">Delete Outlook category</span></span>


<span data-ttu-id="28b41-102">删除指定的 [outlookCategory](../resources/outlookCategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28b41-102">Delete the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28b41-103">权限</span><span class="sxs-lookup"><span data-stu-id="28b41-103">Permissions</span></span>
<span data-ttu-id="28b41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="28b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="28b41-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="28b41-106">Permission type</span></span>      | <span data-ttu-id="28b41-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28b41-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28b41-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28b41-108">Delegated (work or school account)</span></span> | <span data-ttu-id="28b41-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b41-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="28b41-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28b41-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b41-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b41-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="28b41-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="28b41-112">Application</span></span> | <span data-ttu-id="28b41-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b41-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b41-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28b41-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28b41-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="28b41-115">Optional query parameters</span></span>
<span data-ttu-id="28b41-116">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="28b41-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28b41-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="28b41-117">Request headers</span></span>
| <span data-ttu-id="28b41-118">名称</span><span class="sxs-lookup"><span data-stu-id="28b41-118">Name</span></span>      |<span data-ttu-id="28b41-119">说明</span><span class="sxs-lookup"><span data-stu-id="28b41-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28b41-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="28b41-120">Authorization</span></span>  | <span data-ttu-id="28b41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28b41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28b41-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="28b41-123">Request body</span></span>
<span data-ttu-id="28b41-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="28b41-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28b41-125">响应</span><span class="sxs-lookup"><span data-stu-id="28b41-125">Response</span></span>

<span data-ttu-id="28b41-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="28b41-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28b41-128">示例</span><span class="sxs-lookup"><span data-stu-id="28b41-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28b41-129">请求</span><span class="sxs-lookup"><span data-stu-id="28b41-129">Request</span></span>
<span data-ttu-id="28b41-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28b41-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="28b41-131">响应</span><span class="sxs-lookup"><span data-stu-id="28b41-131">Response</span></span>
<span data-ttu-id="28b41-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="28b41-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->