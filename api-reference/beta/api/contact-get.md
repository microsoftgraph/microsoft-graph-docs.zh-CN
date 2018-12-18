---
title: 获取联系人
description: 检索的属性和关系的联系人对象。
author: angelgolfer-ms
ms.openlocfilehash: fceda46729f539081458c1f26c5d385a984ed2d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322923"
---
# <a name="get-contact"></a><span data-ttu-id="89f9c-103">获取联系人</span><span class="sxs-lookup"><span data-stu-id="89f9c-103">Get contact</span></span>

> <span data-ttu-id="89f9c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89f9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89f9c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89f9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89f9c-106">检索的属性和关系的联系人对象。</span><span class="sxs-lookup"><span data-stu-id="89f9c-106">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="89f9c-107">有两种方案，其中应用程序可在另一个用户的联系人文件夹中获取联系人：</span><span class="sxs-lookup"><span data-stu-id="89f9c-107">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="89f9c-108">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="89f9c-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="89f9c-109">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享联系人文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="89f9c-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="89f9c-110">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="89f9c-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="89f9c-111">权限</span><span class="sxs-lookup"><span data-stu-id="89f9c-111">Permissions</span></span>
<span data-ttu-id="89f9c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89f9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89f9c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="89f9c-114">Permission type</span></span>      | <span data-ttu-id="89f9c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89f9c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89f9c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89f9c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="89f9c-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89f9c-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="89f9c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89f9c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89f9c-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89f9c-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="89f9c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="89f9c-120">Application</span></span> | <span data-ttu-id="89f9c-121">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89f9c-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="89f9c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89f9c-122">HTTP request</span></span>
<span data-ttu-id="89f9c-123"><!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)在用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="89f9c-123"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="89f9c-124">[联系人](../resources/contact.md)从用户的顶级[contactFolder](../resources/contactfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="89f9c-124">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="89f9c-125">[联系人](../resources/contact.md) [contactFolder](../resources/mailfolder.md)子文件夹中包含。</span><span class="sxs-lookup"><span data-stu-id="89f9c-125">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="89f9c-126">下面的示例演示一个级别的嵌套，但联系人可以位于子级的子级，依此类推。</span><span class="sxs-lookup"><span data-stu-id="89f9c-126">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89f9c-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89f9c-127">Optional query parameters</span></span>
|<span data-ttu-id="89f9c-128">Name</span><span class="sxs-lookup"><span data-stu-id="89f9c-128">Name</span></span>|<span data-ttu-id="89f9c-129">值</span><span class="sxs-lookup"><span data-stu-id="89f9c-129">Value</span></span>|<span data-ttu-id="89f9c-130">说明</span><span class="sxs-lookup"><span data-stu-id="89f9c-130">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="89f9c-131">$expand</span><span class="sxs-lookup"><span data-stu-id="89f9c-131">$expand</span></span>|<span data-ttu-id="89f9c-132">string</span><span class="sxs-lookup"><span data-stu-id="89f9c-132">string</span></span>|<span data-ttu-id="89f9c-133">要在响应中扩展和添加的关系（以逗号分隔的列表）。</span><span class="sxs-lookup"><span data-stu-id="89f9c-133">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="89f9c-134">查看关系的[联系人](../resources/contact.md)对象所支持的名称。</span><span class="sxs-lookup"><span data-stu-id="89f9c-134">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="89f9c-135">$select</span><span class="sxs-lookup"><span data-stu-id="89f9c-135">$select</span></span>|<span data-ttu-id="89f9c-136">string</span><span class="sxs-lookup"><span data-stu-id="89f9c-136">string</span></span>|<span data-ttu-id="89f9c-137">要在响应中包括的属性的列表（以逗号分隔）。</span><span class="sxs-lookup"><span data-stu-id="89f9c-137">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="89f9c-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="89f9c-138">Request headers</span></span>
| <span data-ttu-id="89f9c-139">标头</span><span class="sxs-lookup"><span data-stu-id="89f9c-139">Header</span></span>       | <span data-ttu-id="89f9c-140">值</span><span class="sxs-lookup"><span data-stu-id="89f9c-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89f9c-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="89f9c-141">Authorization</span></span>  | <span data-ttu-id="89f9c-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89f9c-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89f9c-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="89f9c-144">Request body</span></span>
<span data-ttu-id="89f9c-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89f9c-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89f9c-146">响应</span><span class="sxs-lookup"><span data-stu-id="89f9c-146">Response</span></span>

<span data-ttu-id="89f9c-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89f9c-147">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89f9c-148">示例</span><span class="sxs-lookup"><span data-stu-id="89f9c-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89f9c-149">请求</span><span class="sxs-lookup"><span data-stu-id="89f9c-149">Request</span></span>
<span data-ttu-id="89f9c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89f9c-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
##### <a name="response"></a><span data-ttu-id="89f9c-151">响应</span><span class="sxs-lookup"><span data-stu-id="89f9c-151">Response</span></span>
<span data-ttu-id="89f9c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89f9c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="89f9c-155">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89f9c-155">See also</span></span>

- [<span data-ttu-id="89f9c-156">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="89f9c-156">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="89f9c-157">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="89f9c-157">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->