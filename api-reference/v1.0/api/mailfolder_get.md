# <a name="get-mailfolder"></a><span data-ttu-id="515a7-101">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="515a7-101">Get mailFolder</span></span>

<span data-ttu-id="515a7-102">检索邮件文件夹对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="515a7-102">Retrieve the properties and relationships of a message object.</span></span>


### <a name="get-another-users-message-folder"></a><span data-ttu-id="515a7-103">获取其他用户的邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="515a7-103">Get another user's contact folder</span></span>

<span data-ttu-id="515a7-104">如果拥有应用程序权限，或从某用户获得相应委派[权限](#permissions)，可以获取其他用户的邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="515a7-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="515a7-105">此部分重点介绍了涉及委派权限的方案。</span><span class="sxs-lookup"><span data-stu-id="515a7-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="515a7-106">例如，应用程序已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="515a7-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="515a7-107">假设另一位用户 Garth 与 John 共享了邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="515a7-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="515a7-108">可以在下面的示例查询中指定 Garth 的用户 ID（或用户主体名称），获取此共享文件夹。</span><span class="sxs-lookup"><span data-stu-id="515a7-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/mailFolders/{id}
```

<span data-ttu-id="515a7-109">此功能适用于对各个用户执行的所有受支持 GET 邮件文件夹操作，如下面的 [HTTP 请求](#http-request)部分所列。</span><span class="sxs-lookup"><span data-stu-id="515a7-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="515a7-110">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="515a7-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="515a7-111">如果 Garth 未与 John 共享他的邮件文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="515a7-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="515a7-112">在这种情况下，指定用户 ID 或用户主体名称只适用于获取登录用户的邮件文件夹，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="515a7-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
```

<span data-ttu-id="515a7-113">此功能仅适用于针对以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="515a7-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="515a7-114">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="515a7-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="515a7-115">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="515a7-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="515a7-116">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="515a7-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="515a7-117">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="515a7-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="515a7-118">权限</span><span class="sxs-lookup"><span data-stu-id="515a7-118">Permissions</span></span>
<span data-ttu-id="515a7-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="515a7-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="515a7-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="515a7-121">Permission type</span></span>      | <span data-ttu-id="515a7-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="515a7-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="515a7-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="515a7-123">Delegated (work or school account)</span></span> | <span data-ttu-id="515a7-124">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="515a7-124">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="515a7-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="515a7-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="515a7-126">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="515a7-126">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="515a7-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="515a7-127">Application</span></span> | <span data-ttu-id="515a7-128">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="515a7-128">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="515a7-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="515a7-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="515a7-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="515a7-130">Optional query parameters</span></span>
<span data-ttu-id="515a7-131">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="515a7-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="515a7-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="515a7-132">Request headers</span></span>
| <span data-ttu-id="515a7-133">名称</span><span class="sxs-lookup"><span data-stu-id="515a7-133">Name</span></span>       | <span data-ttu-id="515a7-134">类型</span><span class="sxs-lookup"><span data-stu-id="515a7-134">Type</span></span> | <span data-ttu-id="515a7-135">说明</span><span class="sxs-lookup"><span data-stu-id="515a7-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="515a7-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="515a7-136">Authorization</span></span>  | <span data-ttu-id="515a7-137">string</span><span class="sxs-lookup"><span data-stu-id="515a7-137">string</span></span>  | <span data-ttu-id="515a7-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="515a7-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="515a7-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="515a7-140">Request body</span></span>
<span data-ttu-id="515a7-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="515a7-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="515a7-142">响应</span><span class="sxs-lookup"><span data-stu-id="515a7-142">Response</span></span>

<span data-ttu-id="515a7-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="515a7-143">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="515a7-144">示例</span><span class="sxs-lookup"><span data-stu-id="515a7-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="515a7-145">请求</span><span class="sxs-lookup"><span data-stu-id="515a7-145">Request</span></span>
<span data-ttu-id="515a7-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="515a7-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="515a7-147">响应</span><span class="sxs-lookup"><span data-stu-id="515a7-147">Response</span></span>
<span data-ttu-id="515a7-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="515a7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
