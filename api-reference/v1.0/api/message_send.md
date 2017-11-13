# <a name="message-send"></a><span data-ttu-id="15417-101">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="15417-101">message: send</span></span>

<span data-ttu-id="15417-p101">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="15417-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="15417-105">权限</span><span class="sxs-lookup"><span data-stu-id="15417-105">Permissions</span></span>
<span data-ttu-id="15417-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="15417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="15417-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="15417-108">Permission type</span></span>      | <span data-ttu-id="15417-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15417-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15417-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15417-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15417-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="15417-111">Mail.Send</span></span>    |
|<span data-ttu-id="15417-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15417-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15417-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="15417-113">Mail.Send</span></span>    |
|<span data-ttu-id="15417-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="15417-114">Application</span></span> | <span data-ttu-id="15417-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="15417-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="15417-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15417-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="15417-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="15417-117">Request headers</span></span>
| <span data-ttu-id="15417-118">名称</span><span class="sxs-lookup"><span data-stu-id="15417-118">Name</span></span>       | <span data-ttu-id="15417-119">类型</span><span class="sxs-lookup"><span data-stu-id="15417-119">Type</span></span> | <span data-ttu-id="15417-120">说明</span><span class="sxs-lookup"><span data-stu-id="15417-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15417-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="15417-121">Authorization</span></span>  | <span data-ttu-id="15417-122">string</span><span class="sxs-lookup"><span data-stu-id="15417-122">string</span></span>  | <span data-ttu-id="15417-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15417-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15417-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="15417-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="15417-126">响应</span><span class="sxs-lookup"><span data-stu-id="15417-126">Response</span></span>

<span data-ttu-id="15417-p104">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="15417-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15417-129">示例</span><span class="sxs-lookup"><span data-stu-id="15417-129">Example</span></span>
<span data-ttu-id="15417-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="15417-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="15417-131">请求</span><span class="sxs-lookup"><span data-stu-id="15417-131">Request</span></span>
<span data-ttu-id="15417-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15417-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="15417-133">响应</span><span class="sxs-lookup"><span data-stu-id="15417-133">Response</span></span>

<span data-ttu-id="15417-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="15417-134">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
