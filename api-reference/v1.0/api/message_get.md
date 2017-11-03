# <a name="get-message"></a><span data-ttu-id="2246e-101">获取邮件</span><span class="sxs-lookup"><span data-stu-id="2246e-101">Get message</span></span>

<span data-ttu-id="2246e-102">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2246e-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="2246e-103">由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="2246e-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="2246e-104">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="2246e-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="2246e-105">获取其他用户的邮件文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="2246e-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="2246e-106">如果拥有应用程序权限，或从某用户获得相应委派[权限](#permissions)，可以获取其他用户的邮件文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="2246e-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="2246e-107">此部分重点介绍了涉及委派权限的方案。</span><span class="sxs-lookup"><span data-stu-id="2246e-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="2246e-108">例如，应用程序已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="2246e-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="2246e-109">假设另一位用户 Garth 与 John 共享了邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="2246e-109">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="2246e-110">可以在下面的示例查询中指定 Garth 的用户 ID（或用户主体名称），获取此共享文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="2246e-110">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="2246e-111">此功能适用于对各个用户执行的所有受支持 GET 邮件操作，如下面的 [HTTP 请求](#http-request)部分所列。</span><span class="sxs-lookup"><span data-stu-id="2246e-111">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="2246e-112">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="2246e-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="2246e-113">如果 Garth 未与 John 共享他的邮件文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="2246e-113">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="2246e-114">在这种情况下，指定用户 ID 或用户主体名称只适用于获取登录用户自己的邮件文件夹中的邮件，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="2246e-114">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="2246e-115">此功能仅适用于针对以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="2246e-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="2246e-116">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="2246e-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="2246e-117">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="2246e-117">Contacts and events in shared folders</span></span>
- <span data-ttu-id="2246e-118">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="2246e-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="2246e-119">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="2246e-119">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="2246e-120">权限</span><span class="sxs-lookup"><span data-stu-id="2246e-120">Permissions</span></span>
<span data-ttu-id="2246e-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2246e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2246e-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="2246e-123">Permission type</span></span>      | <span data-ttu-id="2246e-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2246e-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2246e-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2246e-125">Delegated (work or school account)</span></span> | <span data-ttu-id="2246e-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2246e-126">Mail.Read</span></span>    |
|<span data-ttu-id="2246e-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2246e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2246e-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2246e-128">Mail.Read</span></span>    |
|<span data-ttu-id="2246e-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="2246e-129">Application</span></span> | <span data-ttu-id="2246e-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2246e-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2246e-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2246e-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2246e-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2246e-132">Optional query parameters</span></span>
<span data-ttu-id="2246e-133">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2246e-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2246e-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="2246e-134">Request headers</span></span>
| <span data-ttu-id="2246e-135">名称</span><span class="sxs-lookup"><span data-stu-id="2246e-135">Name</span></span>       | <span data-ttu-id="2246e-136">类型</span><span class="sxs-lookup"><span data-stu-id="2246e-136">Type</span></span> | <span data-ttu-id="2246e-137">说明</span><span class="sxs-lookup"><span data-stu-id="2246e-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2246e-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="2246e-138">Authorization</span></span>  | <span data-ttu-id="2246e-139">string</span><span class="sxs-lookup"><span data-stu-id="2246e-139">string</span></span>  | <span data-ttu-id="2246e-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2246e-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2246e-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="2246e-142">Request body</span></span>
<span data-ttu-id="2246e-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2246e-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2246e-144">响应</span><span class="sxs-lookup"><span data-stu-id="2246e-144">Response</span></span>

<span data-ttu-id="2246e-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2246e-145">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2246e-146">示例</span><span class="sxs-lookup"><span data-stu-id="2246e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2246e-147">请求</span><span class="sxs-lookup"><span data-stu-id="2246e-147">Request</span></span>
<span data-ttu-id="2246e-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2246e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="2246e-149">响应</span><span class="sxs-lookup"><span data-stu-id="2246e-149">Response</span></span>
<span data-ttu-id="2246e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2246e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="2246e-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2246e-153">See also</span></span>

- [<span data-ttu-id="2246e-154">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2246e-154">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="2246e-155">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="2246e-155">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
