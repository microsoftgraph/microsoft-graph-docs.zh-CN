# <a name="get-contactfolder"></a><span data-ttu-id="707da-101">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="707da-101">Get contactFolder</span></span>

<span data-ttu-id="707da-102">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="707da-102">Get a contact folder by using the contact folder ID.</span></span>


### <a name="get-another-users-contact-folder"></a><span data-ttu-id="707da-103">获取其他用户的联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="707da-103">Get another user's contact folder</span></span>

<span data-ttu-id="707da-104">如果你具有应用程序权限，或者具有某个用户的相应的委派[权限](#permissions)，则可以获取其他用户的联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="707da-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="707da-105">本部分重点介绍涉及委派权限的应用场景。</span><span class="sxs-lookup"><span data-stu-id="707da-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="707da-106">例如，你的应用已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="707da-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="707da-107">假设另一位用户 Garth 与 John 共享了一个联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="707da-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="707da-108">可以通过在下面所示的查询示例中指定 Garth 的用户 ID（或者用户主体名称）来获取该共享文件夹。</span><span class="sxs-lookup"><span data-stu-id="707da-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contactFolders/{id}
```

<span data-ttu-id="707da-109">此功能适用于对单个用户执行的所有 GET 联系人文件夹操作，如下面的 [HTTP 请求](#http-request)部分所示。</span><span class="sxs-lookup"><span data-stu-id="707da-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="707da-110">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="707da-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="707da-111">如果 Garth 未与 John 共享他的联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="707da-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="707da-112">在这种情况下，指定用户 ID 或用户主体名称只适用于获取已登录用户的联系人文件夹，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="707da-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
```

<span data-ttu-id="707da-113">此功能仅适用于以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="707da-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="707da-114">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="707da-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="707da-115">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="707da-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="707da-116">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="707da-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="707da-117">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="707da-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="707da-118">权限</span><span class="sxs-lookup"><span data-stu-id="707da-118">Permissions</span></span>
<span data-ttu-id="707da-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="707da-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="707da-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="707da-121">Permission type</span></span>      | <span data-ttu-id="707da-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="707da-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="707da-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="707da-123">Delegated (work or school account)</span></span> | <span data-ttu-id="707da-124">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="707da-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="707da-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="707da-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="707da-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="707da-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="707da-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="707da-127">Application</span></span> | <span data-ttu-id="707da-128">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="707da-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="707da-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="707da-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="707da-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="707da-130">Optional query parameters</span></span>
<span data-ttu-id="707da-131">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="707da-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="707da-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="707da-132">Request headers</span></span>
| <span data-ttu-id="707da-133">名称</span><span class="sxs-lookup"><span data-stu-id="707da-133">Name</span></span>       | <span data-ttu-id="707da-134">类型</span><span class="sxs-lookup"><span data-stu-id="707da-134">Type</span></span> | <span data-ttu-id="707da-135">说明</span><span class="sxs-lookup"><span data-stu-id="707da-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="707da-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="707da-136">Authorization</span></span>  | <span data-ttu-id="707da-137">string</span><span class="sxs-lookup"><span data-stu-id="707da-137">string</span></span>  | <span data-ttu-id="707da-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="707da-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="707da-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="707da-140">Request body</span></span>
<span data-ttu-id="707da-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="707da-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="707da-142">响应</span><span class="sxs-lookup"><span data-stu-id="707da-142">Response</span></span>

<span data-ttu-id="707da-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="707da-143">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="707da-144">示例</span><span class="sxs-lookup"><span data-stu-id="707da-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="707da-145">请求</span><span class="sxs-lookup"><span data-stu-id="707da-145">Request</span></span>
<span data-ttu-id="707da-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="707da-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="707da-147">响应</span><span class="sxs-lookup"><span data-stu-id="707da-147">Response</span></span>
<span data-ttu-id="707da-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="707da-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
