# <a name="list-contacts"></a><span data-ttu-id="96c0f-101">列出联系人</span><span class="sxs-lookup"><span data-stu-id="96c0f-101">List contacts</span></span>

<span data-ttu-id="96c0f-102">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="96c0f-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="96c0f-103">获取其他用户的联系人文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="96c0f-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="96c0f-104">如果你具有应用程序权限，或者具有某个用户的相应的委派[权限](#permissions)，则可以获取其他用户的联系人文件夹中的联系人。</span><span class="sxs-lookup"><span data-stu-id="96c0f-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="96c0f-105">本部分重点介绍涉及委派权限的应用场景。</span><span class="sxs-lookup"><span data-stu-id="96c0f-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="96c0f-106">例如，你的应用已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="96c0f-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="96c0f-107">假设另一位用户 Garth 与 John 共享了一个联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="96c0f-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="96c0f-108">可以通过在下面所示的查询示例中指定 Garth 的用户 ID（或者用户主体名称）获取该共享文件夹中的联系人。</span><span class="sxs-lookup"><span data-stu-id="96c0f-108">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

<span data-ttu-id="96c0f-109">此功能适用于对单个用户执行的所有支持的 GET 联系人操作，如下面的 [HTTP 请求](#http-request)部分所示。</span><span class="sxs-lookup"><span data-stu-id="96c0f-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="96c0f-110">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="96c0f-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="96c0f-111">如果 Garth 未与 John 共享他的联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="96c0f-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="96c0f-112">在这种情况下，指定用户 ID 或用户主体名称只适用于获取已登录用户自己的联系人文件夹中的联系人，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="96c0f-112">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

<span data-ttu-id="96c0f-113">此功能仅适用于以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="96c0f-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="96c0f-114">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="96c0f-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="96c0f-115">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="96c0f-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="96c0f-116">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="96c0f-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="96c0f-117">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="96c0f-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="96c0f-118">权限</span><span class="sxs-lookup"><span data-stu-id="96c0f-118">Permissions</span></span>
<span data-ttu-id="96c0f-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="96c0f-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96c0f-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="96c0f-121">Permission type</span></span>      | <span data-ttu-id="96c0f-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96c0f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96c0f-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96c0f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="96c0f-124">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96c0f-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="96c0f-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96c0f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96c0f-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96c0f-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="96c0f-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="96c0f-127">Application</span></span> | <span data-ttu-id="96c0f-128">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96c0f-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96c0f-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96c0f-129">HTTP request</span></span>

<span data-ttu-id="96c0f-130">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="96c0f-130">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="96c0f-131">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="96c0f-131">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96c0f-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96c0f-132">Optional query parameters</span></span>
<span data-ttu-id="96c0f-133">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96c0f-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="96c0f-134">例如，你可以使用 `$filter` 查询参数根据联系人的电子邮件地址的域来过滤联系人：</span><span class="sxs-lookup"><span data-stu-id="96c0f-134">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="96c0f-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="96c0f-135">Request headers</span></span>
| <span data-ttu-id="96c0f-136">标头</span><span class="sxs-lookup"><span data-stu-id="96c0f-136">Header</span></span>       | <span data-ttu-id="96c0f-137">值</span><span class="sxs-lookup"><span data-stu-id="96c0f-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96c0f-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="96c0f-138">Authorization</span></span>  | <span data-ttu-id="96c0f-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96c0f-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96c0f-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96c0f-141">Content-Type</span></span>   | <span data-ttu-id="96c0f-142">application/json</span><span class="sxs-lookup"><span data-stu-id="96c0f-142">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96c0f-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="96c0f-143">Request body</span></span>
<span data-ttu-id="96c0f-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96c0f-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96c0f-145">响应</span><span class="sxs-lookup"><span data-stu-id="96c0f-145">Response</span></span>

<span data-ttu-id="96c0f-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96c0f-146">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96c0f-147">示例</span><span class="sxs-lookup"><span data-stu-id="96c0f-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96c0f-148">请求</span><span class="sxs-lookup"><span data-stu-id="96c0f-148">Request</span></span>
<span data-ttu-id="96c0f-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96c0f-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="96c0f-150">响应</span><span class="sxs-lookup"><span data-stu-id="96c0f-150">Response</span></span>
<span data-ttu-id="96c0f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96c0f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
