# <a name="list-attachments"></a><span data-ttu-id="8ce58-101">列出附件</span><span class="sxs-lookup"><span data-stu-id="8ce58-101">List attachments</span></span>

<span data-ttu-id="8ce58-102">检索附加到邮件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8ce58-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ce58-103">权限</span><span class="sxs-lookup"><span data-stu-id="8ce58-103">Permissions</span></span>
<span data-ttu-id="8ce58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8ce58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ce58-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ce58-106">Permission type</span></span>      | <span data-ttu-id="8ce58-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ce58-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ce58-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ce58-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8ce58-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8ce58-109">Mail.Read</span></span>    |
|<span data-ttu-id="8ce58-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ce58-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ce58-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8ce58-111">Mail.Read</span></span>    |
|<span data-ttu-id="8ce58-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ce58-112">Application</span></span> | <span data-ttu-id="8ce58-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8ce58-113">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ce58-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ce58-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8ce58-115">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="8ce58-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="8ce58-116">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="8ce58-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="8ce58-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="8ce58-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ce58-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8ce58-119">Optional query parameters</span></span>
<span data-ttu-id="8ce58-120">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8ce58-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8ce58-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ce58-121">Request headers</span></span>
| <span data-ttu-id="8ce58-122">名称</span><span class="sxs-lookup"><span data-stu-id="8ce58-122">Name</span></span>       | <span data-ttu-id="8ce58-123">类型</span><span class="sxs-lookup"><span data-stu-id="8ce58-123">Type</span></span> | <span data-ttu-id="8ce58-124">说明</span><span class="sxs-lookup"><span data-stu-id="8ce58-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8ce58-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ce58-125">Authorization</span></span>  | <span data-ttu-id="8ce58-126">string</span><span class="sxs-lookup"><span data-stu-id="8ce58-126">string</span></span>  | <span data-ttu-id="8ce58-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ce58-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ce58-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ce58-129">Request body</span></span>
<span data-ttu-id="8ce58-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8ce58-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ce58-131">响应</span><span class="sxs-lookup"><span data-stu-id="8ce58-131">Response</span></span>

<span data-ttu-id="8ce58-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8ce58-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ce58-133">示例</span><span class="sxs-lookup"><span data-stu-id="8ce58-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ce58-134">请求</span><span class="sxs-lookup"><span data-stu-id="8ce58-134">Request</span></span>
<span data-ttu-id="8ce58-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ce58-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="8ce58-136">响应</span><span class="sxs-lookup"><span data-stu-id="8ce58-136">Response</span></span>
<span data-ttu-id="8ce58-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ce58-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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