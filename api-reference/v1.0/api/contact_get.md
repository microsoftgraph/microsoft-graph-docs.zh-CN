# <a name="get-contact"></a><span data-ttu-id="0fa72-101">获取联系人</span><span class="sxs-lookup"><span data-stu-id="0fa72-101">Get contact</span></span>

<span data-ttu-id="0fa72-102">检索 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fa72-102">Retrieve the properties and relationships of a contact object.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="0fa72-103">获取其他用户的联系人文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="0fa72-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="0fa72-104">如果你具有应用程序权限，或者具有某个用户的相应的委派[权限](#permissions)，则可以获取其他用户的联系人文件夹中的联系人。</span><span class="sxs-lookup"><span data-stu-id="0fa72-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="0fa72-105">本部分重点介绍涉及委派权限的应用场景。</span><span class="sxs-lookup"><span data-stu-id="0fa72-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="0fa72-106">例如，你的应用已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="0fa72-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="0fa72-107">假设另一位用户 Garth 与 John 共享了一个联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="0fa72-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="0fa72-108">可以通过在下面所示的查询示例中指定 Garth 的用户 ID（或者用户主体名称）获取该共享文件夹中的联系人。</span><span class="sxs-lookup"><span data-stu-id="0fa72-108">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts/{id}
```

<span data-ttu-id="0fa72-109">此功能适用于对单个用户执行的所有支持的 GET 联系人操作，如下面的 [HTTP 请求](#http-request)部分所示。</span><span class="sxs-lookup"><span data-stu-id="0fa72-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="0fa72-110">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="0fa72-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="0fa72-111">如果 Garth 未与 John 共享他的联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="0fa72-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="0fa72-112">在这种情况下，指定用户 ID 或用户主体名称只适用于获取已登录用户自身的联系人文件夹中的某个联系人，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="0fa72-112">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}
```

<span data-ttu-id="0fa72-113">此功能仅适用于以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="0fa72-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="0fa72-114">共享联系人文件夹、日历和邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="0fa72-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="0fa72-115">共享文件夹中的联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="0fa72-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="0fa72-116">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="0fa72-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="0fa72-117">此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="0fa72-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="0fa72-118">权限</span><span class="sxs-lookup"><span data-stu-id="0fa72-118">Permissions</span></span>
<span data-ttu-id="0fa72-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa72-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0fa72-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fa72-121">Permission type</span></span>      | <span data-ttu-id="0fa72-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fa72-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fa72-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa72-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0fa72-124">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fa72-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0fa72-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa72-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa72-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fa72-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0fa72-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fa72-127">Application</span></span> | <span data-ttu-id="0fa72-128">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fa72-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa72-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fa72-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0fa72-130">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa72-130">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="0fa72-131">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa72-131">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="0fa72-p106">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="0fa72-p106">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0fa72-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0fa72-134">Optional query parameters</span></span>
|<span data-ttu-id="0fa72-135">Name</span><span class="sxs-lookup"><span data-stu-id="0fa72-135">Name</span></span>|<span data-ttu-id="0fa72-136">值</span><span class="sxs-lookup"><span data-stu-id="0fa72-136">Value</span></span>|<span data-ttu-id="0fa72-137">说明</span><span class="sxs-lookup"><span data-stu-id="0fa72-137">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="0fa72-138">$expand</span><span class="sxs-lookup"><span data-stu-id="0fa72-138">$expand</span></span>|<span data-ttu-id="0fa72-139">string</span><span class="sxs-lookup"><span data-stu-id="0fa72-139">string</span></span>|<span data-ttu-id="0fa72-p107">要在响应中扩展和包括的关系的列表（以逗号分隔）。请参阅支持的名称的 [contact](../resources/contact.md) 对象的关系表。</span><span class="sxs-lookup"><span data-stu-id="0fa72-p107">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="0fa72-142">$select</span><span class="sxs-lookup"><span data-stu-id="0fa72-142">$select</span></span>|<span data-ttu-id="0fa72-143">string</span><span class="sxs-lookup"><span data-stu-id="0fa72-143">string</span></span>|<span data-ttu-id="0fa72-144">要在响应中包括的属性的列表（以逗号分隔）。</span><span class="sxs-lookup"><span data-stu-id="0fa72-144">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0fa72-145">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fa72-145">Request headers</span></span>
| <span data-ttu-id="0fa72-146">标头</span><span class="sxs-lookup"><span data-stu-id="0fa72-146">Header</span></span>       | <span data-ttu-id="0fa72-147">值</span><span class="sxs-lookup"><span data-stu-id="0fa72-147">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fa72-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa72-148">Authorization</span></span>  | <span data-ttu-id="0fa72-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0fa72-p108">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fa72-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fa72-151">Request body</span></span>
<span data-ttu-id="0fa72-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fa72-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fa72-153">响应</span><span class="sxs-lookup"><span data-stu-id="0fa72-153">Response</span></span>

<span data-ttu-id="0fa72-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fa72-154">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fa72-155">示例</span><span class="sxs-lookup"><span data-stu-id="0fa72-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fa72-156">请求</span><span class="sxs-lookup"><span data-stu-id="0fa72-156">Request</span></span>
<span data-ttu-id="0fa72-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fa72-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="0fa72-158">响应</span><span class="sxs-lookup"><span data-stu-id="0fa72-158">Response</span></span>
<span data-ttu-id="0fa72-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0fa72-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "http://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {},
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
