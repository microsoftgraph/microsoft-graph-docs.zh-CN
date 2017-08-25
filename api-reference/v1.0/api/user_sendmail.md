# <a name="send-mail"></a><span data-ttu-id="fac81-101">发送邮件</span><span class="sxs-lookup"><span data-stu-id="fac81-101">Send mail</span></span>

<span data-ttu-id="fac81-p101">发送请求正文中指定的邮件。默认情况下，邮件保存在“已发送邮件”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="fac81-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="fac81-104">可以在同一 **sendMail** 操作调用中包含[文件附件](../resources/fileattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="fac81-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="fac81-105">权限</span><span class="sxs-lookup"><span data-stu-id="fac81-105">Permissions</span></span>
<span data-ttu-id="fac81-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fac81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="fac81-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fac81-108">Permission type</span></span>      | <span data-ttu-id="fac81-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fac81-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fac81-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fac81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fac81-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fac81-111">Mail.Send</span></span>    | 
|<span data-ttu-id="fac81-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fac81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fac81-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fac81-113">Mail.Send</span></span>    | 
|<span data-ttu-id="fac81-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fac81-114">Application</span></span> | <span data-ttu-id="fac81-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fac81-115">Mail.Send</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fac81-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fac81-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="fac81-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fac81-117">Request headers</span></span>
| <span data-ttu-id="fac81-118">标头</span><span class="sxs-lookup"><span data-stu-id="fac81-118">Header</span></span>       | <span data-ttu-id="fac81-119">值</span><span class="sxs-lookup"><span data-stu-id="fac81-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fac81-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fac81-120">Authorization</span></span>  | <span data-ttu-id="fac81-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fac81-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fac81-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fac81-123">Content-Type</span></span>  | <span data-ttu-id="fac81-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fac81-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fac81-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fac81-125">Request body</span></span>
<span data-ttu-id="fac81-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fac81-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fac81-127">参数</span><span class="sxs-lookup"><span data-stu-id="fac81-127">Parameter</span></span>    | <span data-ttu-id="fac81-128">类型</span><span class="sxs-lookup"><span data-stu-id="fac81-128">Type</span></span>   |<span data-ttu-id="fac81-129">说明</span><span class="sxs-lookup"><span data-stu-id="fac81-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fac81-130">Message</span><span class="sxs-lookup"><span data-stu-id="fac81-130">Message</span></span>|[<span data-ttu-id="fac81-131">邮件</span><span class="sxs-lookup"><span data-stu-id="fac81-131">Message</span></span>](../resources/message.md)|<span data-ttu-id="fac81-p104">要发送的邮件。必需。</span><span class="sxs-lookup"><span data-stu-id="fac81-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="fac81-134">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="fac81-134">SaveToSentItems</span></span>|<span data-ttu-id="fac81-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="fac81-135">Boolean</span></span>|<span data-ttu-id="fac81-p105">指示是否将邮件保存在“已发送邮件”文件夹中。仅在该参数为 false 时指定它。默认值为 true。可选。</span><span class="sxs-lookup"><span data-stu-id="fac81-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fac81-139">响应</span><span class="sxs-lookup"><span data-stu-id="fac81-139">Response</span></span>

<span data-ttu-id="fac81-p106">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fac81-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fac81-142">示例</span><span class="sxs-lookup"><span data-stu-id="fac81-142">Example</span></span>
<span data-ttu-id="fac81-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fac81-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fac81-144">请求</span><span class="sxs-lookup"><span data-stu-id="fac81-144">Request</span></span>
<span data-ttu-id="fac81-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fac81-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response"></a><span data-ttu-id="fac81-146">响应</span><span class="sxs-lookup"><span data-stu-id="fac81-146">Response</span></span>
<span data-ttu-id="fac81-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fac81-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
