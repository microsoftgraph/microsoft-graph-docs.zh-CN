---
title: 获取联系人
description: 检索 contact 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 79f70fb7b7f591e7d17c1286e2900848a415d653
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327617"
---
# <a name="get-contact"></a><span data-ttu-id="3d192-103">获取联系人</span><span class="sxs-lookup"><span data-stu-id="3d192-103">Get contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d192-104">检索 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d192-104">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="3d192-105">在以下两种情况下, 应用可以在其他用户的 "联系人" 文件夹中获取联系人:</span><span class="sxs-lookup"><span data-stu-id="3d192-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="3d192-106">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="3d192-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="3d192-107">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="3d192-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="3d192-108">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="3d192-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="3d192-109">权限</span><span class="sxs-lookup"><span data-stu-id="3d192-109">Permissions</span></span>
<span data-ttu-id="3d192-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d192-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d192-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d192-112">Permission type</span></span>      | <span data-ttu-id="3d192-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d192-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d192-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d192-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3d192-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d192-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3d192-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d192-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d192-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d192-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3d192-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d192-118">Application</span></span> | <span data-ttu-id="3d192-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d192-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d192-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d192-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3d192-121">用户邮箱中的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="3d192-121">A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="3d192-122">来自用户的顶级[contactFolder](../resources/contactfolder.md)的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="3d192-122">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="3d192-123">[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="3d192-123">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="3d192-124">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="3d192-124">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d192-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3d192-125">Optional query parameters</span></span>
|<span data-ttu-id="3d192-126">名称</span><span class="sxs-lookup"><span data-stu-id="3d192-126">Name</span></span>|<span data-ttu-id="3d192-127">值</span><span class="sxs-lookup"><span data-stu-id="3d192-127">Value</span></span>|<span data-ttu-id="3d192-128">说明</span><span class="sxs-lookup"><span data-stu-id="3d192-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="3d192-129">$expand</span><span class="sxs-lookup"><span data-stu-id="3d192-129">$expand</span></span>|<span data-ttu-id="3d192-130">string</span><span class="sxs-lookup"><span data-stu-id="3d192-130">string</span></span>|<span data-ttu-id="3d192-131">要在响应中扩展和添加的关系（以逗号分隔的列表）。</span><span class="sxs-lookup"><span data-stu-id="3d192-131">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="3d192-132">有关受支持的名称, 请参阅[contact](../resources/contact.md)对象的关系表。</span><span class="sxs-lookup"><span data-stu-id="3d192-132">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="3d192-133">$select</span><span class="sxs-lookup"><span data-stu-id="3d192-133">$select</span></span>|<span data-ttu-id="3d192-134">string</span><span class="sxs-lookup"><span data-stu-id="3d192-134">string</span></span>|<span data-ttu-id="3d192-135">要在响应中包括的属性的列表（以逗号分隔）。</span><span class="sxs-lookup"><span data-stu-id="3d192-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3d192-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d192-136">Request headers</span></span>
| <span data-ttu-id="3d192-137">标头</span><span class="sxs-lookup"><span data-stu-id="3d192-137">Header</span></span>       | <span data-ttu-id="3d192-138">值</span><span class="sxs-lookup"><span data-stu-id="3d192-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3d192-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d192-139">Authorization</span></span>  | <span data-ttu-id="3d192-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d192-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3d192-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d192-142">Request body</span></span>
<span data-ttu-id="3d192-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d192-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d192-144">响应</span><span class="sxs-lookup"><span data-stu-id="3d192-144">Response</span></span>

<span data-ttu-id="3d192-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d192-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d192-146">示例</span><span class="sxs-lookup"><span data-stu-id="3d192-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d192-147">请求</span><span class="sxs-lookup"><span data-stu-id="3d192-147">Request</span></span>
<span data-ttu-id="3d192-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d192-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
##### <a name="response"></a><span data-ttu-id="3d192-149">响应</span><span class="sxs-lookup"><span data-stu-id="3d192-149">Response</span></span>
<span data-ttu-id="3d192-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d192-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3d192-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3d192-153">See also</span></span>

- [<span data-ttu-id="3d192-154">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3d192-154">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3d192-155">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3d192-155">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "suppressions": []
}
-->
