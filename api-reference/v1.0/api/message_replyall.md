# <a name="message-replyall"></a><span data-ttu-id="c1a26-101">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="c1a26-101">message: replyAll</span></span>

<span data-ttu-id="c1a26-p101">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="c1a26-p101">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a26-104">权限</span><span class="sxs-lookup"><span data-stu-id="c1a26-104">Permissions</span></span>
<span data-ttu-id="c1a26-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c1a26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1a26-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1a26-107">Permission type</span></span>      | <span data-ttu-id="c1a26-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1a26-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1a26-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a26-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c1a26-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c1a26-110">Mail.Send</span></span>    |
|<span data-ttu-id="c1a26-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a26-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a26-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c1a26-112">Mail.Send</span></span>    |
|<span data-ttu-id="c1a26-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1a26-113">Application</span></span> | <span data-ttu-id="c1a26-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c1a26-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1a26-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1a26-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="c1a26-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1a26-116">Request headers</span></span>
| <span data-ttu-id="c1a26-117">名称</span><span class="sxs-lookup"><span data-stu-id="c1a26-117">Name</span></span>       | <span data-ttu-id="c1a26-118">类型</span><span class="sxs-lookup"><span data-stu-id="c1a26-118">Type</span></span> | <span data-ttu-id="c1a26-119">说明</span><span class="sxs-lookup"><span data-stu-id="c1a26-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c1a26-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1a26-120">Authorization</span></span>  | <span data-ttu-id="c1a26-121">string</span><span class="sxs-lookup"><span data-stu-id="c1a26-121">string</span></span>  | <span data-ttu-id="c1a26-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1a26-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1a26-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1a26-124">Content-Type</span></span> | <span data-ttu-id="c1a26-125">string</span><span class="sxs-lookup"><span data-stu-id="c1a26-125">string</span></span>  | <span data-ttu-id="c1a26-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="c1a26-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1a26-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1a26-128">Request body</span></span>
<span data-ttu-id="c1a26-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c1a26-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1a26-130">参数</span><span class="sxs-lookup"><span data-stu-id="c1a26-130">Parameter</span></span>    | <span data-ttu-id="c1a26-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1a26-131">Type</span></span>   |<span data-ttu-id="c1a26-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1a26-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1a26-133">注释</span><span class="sxs-lookup"><span data-stu-id="c1a26-133">comment</span></span>|<span data-ttu-id="c1a26-134">String</span><span class="sxs-lookup"><span data-stu-id="c1a26-134">String</span></span>|<span data-ttu-id="c1a26-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="c1a26-p105">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="c1a26-137">响应</span><span class="sxs-lookup"><span data-stu-id="c1a26-137">Response</span></span>

<span data-ttu-id="c1a26-p106">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c1a26-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a26-140">示例</span><span class="sxs-lookup"><span data-stu-id="c1a26-140">Example</span></span>
<span data-ttu-id="c1a26-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c1a26-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1a26-142">请求</span><span class="sxs-lookup"><span data-stu-id="c1a26-142">Request</span></span>
<span data-ttu-id="c1a26-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1a26-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="c1a26-144">响应</span><span class="sxs-lookup"><span data-stu-id="c1a26-144">Response</span></span>
<span data-ttu-id="c1a26-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c1a26-145">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
