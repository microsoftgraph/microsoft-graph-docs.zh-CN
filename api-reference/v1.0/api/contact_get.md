# <a name="get-contact"></a><span data-ttu-id="a1c31-101">获取联系人</span><span class="sxs-lookup"><span data-stu-id="a1c31-101">Get contact</span></span>

<span data-ttu-id="a1c31-102">检索 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1c31-102">Retrieve the properties and relationships of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1c31-103">权限</span><span class="sxs-lookup"><span data-stu-id="a1c31-103">Permissions</span></span>
<span data-ttu-id="a1c31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a1c31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1c31-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1c31-106">Permission type</span></span>      | <span data-ttu-id="a1c31-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1c31-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a1c31-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1c31-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a1c31-109">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c31-109">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="a1c31-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1c31-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c31-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c31-111">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="a1c31-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1c31-112">Application</span></span> | <span data-ttu-id="a1c31-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c31-113">Contacts.Read, Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a1c31-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1c31-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a1c31-115">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="a1c31-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="a1c31-116">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="a1c31-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="a1c31-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="a1c31-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1c31-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1c31-119">Optional query parameters</span></span>
|<span data-ttu-id="a1c31-120">Name</span><span class="sxs-lookup"><span data-stu-id="a1c31-120">Name</span></span>|<span data-ttu-id="a1c31-121">值</span><span class="sxs-lookup"><span data-stu-id="a1c31-121">Value</span></span>|<span data-ttu-id="a1c31-122">说明</span><span class="sxs-lookup"><span data-stu-id="a1c31-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="a1c31-123">$expand</span><span class="sxs-lookup"><span data-stu-id="a1c31-123">$expand</span></span>|<span data-ttu-id="a1c31-124">string</span><span class="sxs-lookup"><span data-stu-id="a1c31-124">string</span></span>|<span data-ttu-id="a1c31-p103">要在响应中扩展和包括的关系的列表（以逗号分隔）。请参阅支持的名称的 [contact](../resources/contact.md) 对象的关系表。</span><span class="sxs-lookup"><span data-stu-id="a1c31-p103">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="a1c31-127">$select</span><span class="sxs-lookup"><span data-stu-id="a1c31-127">$select</span></span>|<span data-ttu-id="a1c31-128">string</span><span class="sxs-lookup"><span data-stu-id="a1c31-128">string</span></span>|<span data-ttu-id="a1c31-129">要在响应中包括的属性的列表（以逗号分隔）。</span><span class="sxs-lookup"><span data-stu-id="a1c31-129">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a1c31-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1c31-130">Request headers</span></span>
| <span data-ttu-id="a1c31-131">标头</span><span class="sxs-lookup"><span data-stu-id="a1c31-131">Header</span></span>       | <span data-ttu-id="a1c31-132">值</span><span class="sxs-lookup"><span data-stu-id="a1c31-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a1c31-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1c31-133">Authorization</span></span>  | <span data-ttu-id="a1c31-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1c31-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1c31-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1c31-136">Request body</span></span>
<span data-ttu-id="a1c31-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1c31-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1c31-138">响应</span><span class="sxs-lookup"><span data-stu-id="a1c31-138">Response</span></span>

<span data-ttu-id="a1c31-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1c31-139">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1c31-140">示例</span><span class="sxs-lookup"><span data-stu-id="a1c31-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1c31-141">请求</span><span class="sxs-lookup"><span data-stu-id="a1c31-141">Request</span></span>
<span data-ttu-id="a1c31-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1c31-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="a1c31-143">响应</span><span class="sxs-lookup"><span data-stu-id="a1c31-143">Response</span></span>
<span data-ttu-id="a1c31-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1c31-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
