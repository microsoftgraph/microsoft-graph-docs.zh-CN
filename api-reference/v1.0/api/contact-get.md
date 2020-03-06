---
title: 获取联系人
description: 检索 contact 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6ffff6875ad3b874d9c15551c6c981ac7881f71d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518299"
---
# <a name="get-contact"></a><span data-ttu-id="01f21-103">获取联系人</span><span class="sxs-lookup"><span data-stu-id="01f21-103">Get contact</span></span>

<span data-ttu-id="01f21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01f21-105">检索 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01f21-105">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="01f21-106">在以下两种情况下，应用可以在其他用户的 "联系人" 文件夹中获取联系人：</span><span class="sxs-lookup"><span data-stu-id="01f21-106">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="01f21-107">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="01f21-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="01f21-108">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="01f21-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="01f21-109">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="01f21-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="01f21-110">权限</span><span class="sxs-lookup"><span data-stu-id="01f21-110">Permissions</span></span>
<span data-ttu-id="01f21-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01f21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f21-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="01f21-113">Permission type</span></span>      | <span data-ttu-id="01f21-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01f21-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f21-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01f21-115">Delegated (work or school account)</span></span> | <span data-ttu-id="01f21-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f21-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="01f21-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01f21-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f21-118">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f21-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="01f21-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="01f21-119">Application</span></span> | <span data-ttu-id="01f21-120">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f21-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f21-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01f21-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="01f21-122">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="01f21-122">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="01f21-123">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="01f21-123">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="01f21-p103">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="01f21-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01f21-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01f21-126">Optional query parameters</span></span>
|<span data-ttu-id="01f21-127">名称</span><span class="sxs-lookup"><span data-stu-id="01f21-127">Name</span></span>|<span data-ttu-id="01f21-128">值</span><span class="sxs-lookup"><span data-stu-id="01f21-128">Value</span></span>|<span data-ttu-id="01f21-129">说明</span><span class="sxs-lookup"><span data-stu-id="01f21-129">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="01f21-130">$expand</span><span class="sxs-lookup"><span data-stu-id="01f21-130">$expand</span></span>|<span data-ttu-id="01f21-131">string</span><span class="sxs-lookup"><span data-stu-id="01f21-131">string</span></span>|<span data-ttu-id="01f21-p104">要在响应中扩展和包括的关系的列表（以逗号分隔）。请参阅支持的名称的 [contact](../resources/contact.md) 对象的关系表。</span><span class="sxs-lookup"><span data-stu-id="01f21-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="01f21-134">$select</span><span class="sxs-lookup"><span data-stu-id="01f21-134">$select</span></span>|<span data-ttu-id="01f21-135">string</span><span class="sxs-lookup"><span data-stu-id="01f21-135">string</span></span>|<span data-ttu-id="01f21-136">要在响应中包括的属性的列表（以逗号分隔）。</span><span class="sxs-lookup"><span data-stu-id="01f21-136">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="01f21-137">请求头</span><span class="sxs-lookup"><span data-stu-id="01f21-137">Request headers</span></span>
| <span data-ttu-id="01f21-138">标头</span><span class="sxs-lookup"><span data-stu-id="01f21-138">Header</span></span>       | <span data-ttu-id="01f21-139">值</span><span class="sxs-lookup"><span data-stu-id="01f21-139">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01f21-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f21-140">Authorization</span></span>  | <span data-ttu-id="01f21-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01f21-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01f21-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="01f21-143">Request body</span></span>
<span data-ttu-id="01f21-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01f21-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f21-145">响应</span><span class="sxs-lookup"><span data-stu-id="01f21-145">Response</span></span>

<span data-ttu-id="01f21-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01f21-146">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01f21-147">示例</span><span class="sxs-lookup"><span data-stu-id="01f21-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01f21-148">请求</span><span class="sxs-lookup"><span data-stu-id="01f21-148">Request</span></span>
<span data-ttu-id="01f21-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01f21-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01f21-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="01f21-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="01f21-151">C#</span><span class="sxs-lookup"><span data-stu-id="01f21-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01f21-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01f21-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01f21-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01f21-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01f21-154">Java</span><span class="sxs-lookup"><span data-stu-id="01f21-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01f21-155">响应</span><span class="sxs-lookup"><span data-stu-id="01f21-155">Response</span></span>
<span data-ttu-id="01f21-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01f21-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "https://www.contoso.com",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
