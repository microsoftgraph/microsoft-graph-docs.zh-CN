---
title: 获取联系人
description: 检索 contact 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cd49e7ecb48274230049afa13774e67f7b38b23f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321671"
---
# <a name="get-contact"></a><span data-ttu-id="17781-103">获取联系人</span><span class="sxs-lookup"><span data-stu-id="17781-103">Get contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17781-104">检索 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17781-104">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="17781-105">在以下两种情况下, 应用可以在其他用户的 "联系人" 文件夹中获取联系人:</span><span class="sxs-lookup"><span data-stu-id="17781-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="17781-106">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="17781-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="17781-107">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="17781-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="17781-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="17781-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="17781-109">权限</span><span class="sxs-lookup"><span data-stu-id="17781-109">Permissions</span></span>
<span data-ttu-id="17781-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17781-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17781-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="17781-112">Permission type</span></span>      | <span data-ttu-id="17781-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17781-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17781-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17781-114">Delegated (work or school account)</span></span> | <span data-ttu-id="17781-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17781-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="17781-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17781-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17781-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17781-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="17781-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="17781-118">Application</span></span> | <span data-ttu-id="17781-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17781-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="17781-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17781-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="17781-121">用户邮箱中的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="17781-121">A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="17781-122">来自用户的顶级[contactFolder](../resources/contactfolder.md)的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="17781-122">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="17781-123">[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="17781-123">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="17781-124">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="17781-124">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17781-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17781-125">Optional query parameters</span></span>
|<span data-ttu-id="17781-126">名称</span><span class="sxs-lookup"><span data-stu-id="17781-126">Name</span></span>|<span data-ttu-id="17781-127">值</span><span class="sxs-lookup"><span data-stu-id="17781-127">Value</span></span>|<span data-ttu-id="17781-128">说明</span><span class="sxs-lookup"><span data-stu-id="17781-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="17781-129">$expand</span><span class="sxs-lookup"><span data-stu-id="17781-129">$expand</span></span>|<span data-ttu-id="17781-130">string</span><span class="sxs-lookup"><span data-stu-id="17781-130">string</span></span>|<span data-ttu-id="17781-131">要在响应中扩展和添加的关系（以逗号分隔的列表）。</span><span class="sxs-lookup"><span data-stu-id="17781-131">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="17781-132">有关受支持的名称, 请参阅[contact](../resources/contact.md)对象的关系表。</span><span class="sxs-lookup"><span data-stu-id="17781-132">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="17781-133">$select</span><span class="sxs-lookup"><span data-stu-id="17781-133">$select</span></span>|<span data-ttu-id="17781-134">string</span><span class="sxs-lookup"><span data-stu-id="17781-134">string</span></span>|<span data-ttu-id="17781-135">要在响应中包括的属性的列表（以逗号分隔）。</span><span class="sxs-lookup"><span data-stu-id="17781-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="17781-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="17781-136">Request headers</span></span>
| <span data-ttu-id="17781-137">标头</span><span class="sxs-lookup"><span data-stu-id="17781-137">Header</span></span>       | <span data-ttu-id="17781-138">值</span><span class="sxs-lookup"><span data-stu-id="17781-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17781-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="17781-139">Authorization</span></span>  | <span data-ttu-id="17781-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17781-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17781-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="17781-142">Request body</span></span>
<span data-ttu-id="17781-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17781-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17781-144">响应</span><span class="sxs-lookup"><span data-stu-id="17781-144">Response</span></span>

<span data-ttu-id="17781-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17781-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17781-146">示例</span><span class="sxs-lookup"><span data-stu-id="17781-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17781-147">请求</span><span class="sxs-lookup"><span data-stu-id="17781-147">Request</span></span>
<span data-ttu-id="17781-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17781-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17781-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="17781-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17781-150">C#</span><span class="sxs-lookup"><span data-stu-id="17781-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17781-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17781-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17781-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="17781-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="17781-153">Java</span><span class="sxs-lookup"><span data-stu-id="17781-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17781-154">响应</span><span class="sxs-lookup"><span data-stu-id="17781-154">Response</span></span>
<span data-ttu-id="17781-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17781-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com",
      "type": "unknown"
    },
    {
      "name": "Garth",
      "address": "garth@contoso.onmicrosoft.com",
      "type": "personal"
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
  "assistantName": null,
  "manager": null,
  "phones": [{
    "type": "business",
    "number": "+1 918 555 0101"
  }],
  "postalAddresses": [{
    "type": "business",
    "postOfficeBox": "P.O. Box 100",
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "countryOrRegion": "USA",
    "postalCode": "98121"
  }],
  "spouseName": null,
  "personalNotes": null,
  "children": [], 
  "gender": null,
  "websites": [{
      "type": "work",
      "address": "https://www.contoso.com",
      "name": "Contoso"
  }],
  "weddingAnniversary": null
}
```

## <a name="see-also"></a><span data-ttu-id="17781-158">另请参阅</span><span class="sxs-lookup"><span data-stu-id="17781-158">See also</span></span>

- [<span data-ttu-id="17781-159">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="17781-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="17781-160">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="17781-160">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
