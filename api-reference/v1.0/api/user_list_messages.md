# <a name="list-messages"></a><span data-ttu-id="c157d-101">List messages</span><span class="sxs-lookup"><span data-stu-id="c157d-101">List messages</span></span>

<span data-ttu-id="c157d-102">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="c157d-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="c157d-103">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="c157d-103">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="c157d-104">获取其他用户的邮件文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="c157d-104">Get messages in another user's message folder</span></span>

<span data-ttu-id="c157d-105">如果拥有应用程序权限，或从某用户获得相应委派[权限](#permissions)，可以获取其他用户的邮件文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="c157d-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="c157d-106">此部分重点介绍了涉及委派权限的方案。</span><span class="sxs-lookup"><span data-stu-id="c157d-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="c157d-107">例如，应用程序已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="c157d-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="c157d-108">假设另一位用户 Garth 与 John 共享了邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="c157d-108">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="c157d-109">可以在下面的示例查询中指定 Garth 的用户 ID（或用户主体名称），获取此共享文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="c157d-109">You can get the messages in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

<span data-ttu-id="c157d-110">此功能适用于对各个用户执行的所有受支持 GET 邮件操作，如下面的 [HTTP 请求](#http-request)部分所列。</span><span class="sxs-lookup"><span data-stu-id="c157d-110">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="c157d-111">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="c157d-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="c157d-112">如果 Garth 未与 John 共享他的邮件文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="c157d-112">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="c157d-113">在这种情况下，指定用户 ID 或用户主体名称只适用于获取登录用户自己的邮件文件夹中的邮件，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="c157d-113">In such cases, specifying a user ID or user principal name only works for getting messages in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

<span data-ttu-id="c157d-114">此功能仅适用于针对以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="c157d-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="c157d-115">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="c157d-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="c157d-116">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="c157d-116">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="c157d-117">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="c157d-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="c157d-118">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="c157d-118">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="c157d-119">权限</span><span class="sxs-lookup"><span data-stu-id="c157d-119">Permissions</span></span>
<span data-ttu-id="c157d-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c157d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c157d-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="c157d-122">Permission type</span></span>      | <span data-ttu-id="c157d-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c157d-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c157d-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c157d-124">Delegated (work or school account)</span></span> | <span data-ttu-id="c157d-125">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c157d-125">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c157d-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c157d-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c157d-127">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c157d-127">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c157d-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="c157d-128">Application</span></span> | <span data-ttu-id="c157d-129">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c157d-129">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c157d-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c157d-130">HTTP request</span></span>

<span data-ttu-id="c157d-131">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c157d-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="c157d-132">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c157d-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c157d-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c157d-133">Optional query parameters</span></span>
<span data-ttu-id="c157d-134">此方法支持 [OData 查询参数]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c157d-134">This method supports the [OData Query Parameters]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c157d-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="c157d-135">Request headers</span></span>
| <span data-ttu-id="c157d-136">名称</span><span class="sxs-lookup"><span data-stu-id="c157d-136">Name</span></span>       | <span data-ttu-id="c157d-137">类型</span><span class="sxs-lookup"><span data-stu-id="c157d-137">Type</span></span> | <span data-ttu-id="c157d-138">说明</span><span class="sxs-lookup"><span data-stu-id="c157d-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c157d-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="c157d-139">Authorization</span></span>  | <span data-ttu-id="c157d-140">string</span><span class="sxs-lookup"><span data-stu-id="c157d-140">string</span></span>  | <span data-ttu-id="c157d-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="c157d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c157d-143">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="c157d-143">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="c157d-144">string</span><span class="sxs-lookup"><span data-stu-id="c157d-144">string</span></span> | <span data-ttu-id="c157d-145">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="c157d-145">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="c157d-146">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="c157d-146">Values can be "text" or "html".</span></span> <span data-ttu-id="c157d-147">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="c157d-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="c157d-148">可选。</span><span class="sxs-lookup"><span data-stu-id="c157d-148">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c157d-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="c157d-149">Request body</span></span>
<span data-ttu-id="c157d-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c157d-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c157d-151">响应</span><span class="sxs-lookup"><span data-stu-id="c157d-151">Response</span></span>

<span data-ttu-id="c157d-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c157d-152">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="c157d-153">此请求的默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="c157d-153">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="c157d-154">示例</span><span class="sxs-lookup"><span data-stu-id="c157d-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c157d-155">请求</span><span class="sxs-lookup"><span data-stu-id="c157d-155">Request</span></span>
<span data-ttu-id="c157d-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c157d-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="c157d-157">响应</span><span class="sxs-lookup"><span data-stu-id="c157d-157">Response</span></span>
<span data-ttu-id="c157d-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c157d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
