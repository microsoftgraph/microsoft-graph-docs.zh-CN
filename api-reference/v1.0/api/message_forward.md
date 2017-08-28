# <a name="message-forward"></a><span data-ttu-id="4bc3c-101">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="4bc3c-101">message: forward</span></span>

<span data-ttu-id="4bc3c-p101">转发邮件。邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bc3c-104">权限</span><span class="sxs-lookup"><span data-stu-id="4bc3c-104">Permissions</span></span>
<span data-ttu-id="4bc3c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bc3c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bc3c-107">Permission type</span></span>      | <span data-ttu-id="4bc3c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bc3c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bc3c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bc3c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4bc3c-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4bc3c-110">Mail.Send</span></span>    |
|<span data-ttu-id="4bc3c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bc3c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bc3c-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4bc3c-112">Mail.Send</span></span>    |
|<span data-ttu-id="4bc3c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bc3c-113">Application</span></span> | <span data-ttu-id="4bc3c-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4bc3c-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bc3c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bc3c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="4bc3c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bc3c-116">Request headers</span></span>
| <span data-ttu-id="4bc3c-117">名称</span><span class="sxs-lookup"><span data-stu-id="4bc3c-117">Name</span></span>       | <span data-ttu-id="4bc3c-118">类型</span><span class="sxs-lookup"><span data-stu-id="4bc3c-118">Type</span></span> | <span data-ttu-id="4bc3c-119">说明</span><span class="sxs-lookup"><span data-stu-id="4bc3c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bc3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bc3c-120">Authorization</span></span>  | <span data-ttu-id="4bc3c-121">string</span><span class="sxs-lookup"><span data-stu-id="4bc3c-121">string</span></span>  | <span data-ttu-id="4bc3c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bc3c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4bc3c-124">Content-Type</span></span> | <span data-ttu-id="4bc3c-125">string</span><span class="sxs-lookup"><span data-stu-id="4bc3c-125">string</span></span>  | <span data-ttu-id="4bc3c-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bc3c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bc3c-128">Request body</span></span>
<span data-ttu-id="4bc3c-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bc3c-130">参数</span><span class="sxs-lookup"><span data-stu-id="4bc3c-130">Parameter</span></span>    | <span data-ttu-id="4bc3c-131">类型</span><span class="sxs-lookup"><span data-stu-id="4bc3c-131">Type</span></span>   |<span data-ttu-id="4bc3c-132">说明</span><span class="sxs-lookup"><span data-stu-id="4bc3c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bc3c-133">注释</span><span class="sxs-lookup"><span data-stu-id="4bc3c-133">comment</span></span>|<span data-ttu-id="4bc3c-134">String</span><span class="sxs-lookup"><span data-stu-id="4bc3c-134">String</span></span>|<span data-ttu-id="4bc3c-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="4bc3c-137">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4bc3c-137">toRecipients</span></span>|<span data-ttu-id="4bc3c-138">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="4bc3c-138">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="4bc3c-139">收件人列表</span><span class="sxs-lookup"><span data-stu-id="4bc3c-139">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="4bc3c-140">响应</span><span class="sxs-lookup"><span data-stu-id="4bc3c-140">Response</span></span>

<span data-ttu-id="4bc3c-p106">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc3c-143">示例</span><span class="sxs-lookup"><span data-stu-id="4bc3c-143">Example</span></span>
<span data-ttu-id="4bc3c-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4bc3c-145">请求</span><span class="sxs-lookup"><span data-stu-id="4bc3c-145">Request</span></span>
<span data-ttu-id="4bc3c-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="4bc3c-147">响应</span><span class="sxs-lookup"><span data-stu-id="4bc3c-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="4bc3c-148">响应</span><span class="sxs-lookup"><span data-stu-id="4bc3c-148">Response</span></span>
<span data-ttu-id="4bc3c-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4bc3c-149">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
