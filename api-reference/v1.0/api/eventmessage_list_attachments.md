# <a name="list-attachments"></a><span data-ttu-id="e20de-101">列出附件</span><span class="sxs-lookup"><span data-stu-id="e20de-101">List attachments</span></span>

<span data-ttu-id="e20de-102">检索 attachment 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e20de-102">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e20de-103">权限</span><span class="sxs-lookup"><span data-stu-id="e20de-103">Permissions</span></span>
<span data-ttu-id="e20de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e20de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e20de-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="e20de-106">Permission type</span></span>      | <span data-ttu-id="e20de-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e20de-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e20de-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e20de-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e20de-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e20de-109">Mail.Read</span></span>    |
|<span data-ttu-id="e20de-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e20de-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e20de-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e20de-111">Mail.Read</span></span>    |
|<span data-ttu-id="e20de-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e20de-112">Application</span></span> | <span data-ttu-id="e20de-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e20de-113">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e20de-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e20de-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e20de-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e20de-115">Optional query parameters</span></span>
<span data-ttu-id="e20de-116">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e20de-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e20de-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e20de-117">Request headers</span></span>
| <span data-ttu-id="e20de-118">名称</span><span class="sxs-lookup"><span data-stu-id="e20de-118">Name</span></span>       | <span data-ttu-id="e20de-119">类型</span><span class="sxs-lookup"><span data-stu-id="e20de-119">Type</span></span> | <span data-ttu-id="e20de-120">说明</span><span class="sxs-lookup"><span data-stu-id="e20de-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e20de-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e20de-121">Authorization</span></span>  | <span data-ttu-id="e20de-122">string</span><span class="sxs-lookup"><span data-stu-id="e20de-122">string</span></span>  | <span data-ttu-id="e20de-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e20de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e20de-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e20de-125">Request body</span></span>
<span data-ttu-id="e20de-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e20de-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e20de-127">响应</span><span class="sxs-lookup"><span data-stu-id="e20de-127">Response</span></span>

<span data-ttu-id="e20de-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e20de-128">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e20de-129">示例</span><span class="sxs-lookup"><span data-stu-id="e20de-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e20de-130">请求</span><span class="sxs-lookup"><span data-stu-id="e20de-130">Request</span></span>
<span data-ttu-id="e20de-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e20de-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="e20de-132">响应</span><span class="sxs-lookup"><span data-stu-id="e20de-132">Response</span></span>
<span data-ttu-id="e20de-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e20de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
