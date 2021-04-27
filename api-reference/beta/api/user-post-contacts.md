---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0926ae86158b2a3bc521230ff3303fe609cb5f20
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053333"
---
# <a name="create-contact"></a><span data-ttu-id="09dd7-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="09dd7-103">Create Contact</span></span>

<span data-ttu-id="09dd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09dd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09dd7-105">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="09dd7-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="09dd7-106">权限</span><span class="sxs-lookup"><span data-stu-id="09dd7-106">Permissions</span></span>
<span data-ttu-id="09dd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09dd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09dd7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09dd7-109">Permission type</span></span>      | <span data-ttu-id="09dd7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09dd7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09dd7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09dd7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="09dd7-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09dd7-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="09dd7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09dd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09dd7-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09dd7-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="09dd7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09dd7-115">Application</span></span> | <span data-ttu-id="09dd7-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09dd7-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="09dd7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09dd7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="09dd7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09dd7-118">Request headers</span></span>
| <span data-ttu-id="09dd7-119">标头</span><span class="sxs-lookup"><span data-stu-id="09dd7-119">Header</span></span>       | <span data-ttu-id="09dd7-120">值</span><span class="sxs-lookup"><span data-stu-id="09dd7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09dd7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09dd7-121">Authorization</span></span>  | <span data-ttu-id="09dd7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09dd7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09dd7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09dd7-124">Content-Type</span></span>  | <span data-ttu-id="09dd7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09dd7-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09dd7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="09dd7-126">Request body</span></span>
<span data-ttu-id="09dd7-127">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09dd7-127">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="09dd7-128">响应</span><span class="sxs-lookup"><span data-stu-id="09dd7-128">Response</span></span>

<span data-ttu-id="09dd7-129">如果成功，此方法在 `201 Created` 响应正文中返回 [响应](../resources/contact.md) 代码和 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="09dd7-129">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09dd7-130">示例</span><span class="sxs-lookup"><span data-stu-id="09dd7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09dd7-131">请求</span><span class="sxs-lookup"><span data-stu-id="09dd7-131">Request</span></span>
<span data-ttu-id="09dd7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09dd7-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09dd7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="09dd7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@contoso.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "personal"
    },
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "other",
      "otherLabel": "Volunteer work"
    }
  ],
  "phones" : [
    {
      "number": "+1 732 555 0102",
      "type": "business"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="09dd7-134">C#</span><span class="sxs-lookup"><span data-stu-id="09dd7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09dd7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09dd7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09dd7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09dd7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09dd7-137">Java</span><span class="sxs-lookup"><span data-stu-id="09dd7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="09dd7-138">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09dd7-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="09dd7-139">响应</span><span class="sxs-lookup"><span data-stu-id="09dd7-139">Response</span></span>
<span data-ttu-id="09dd7-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="09dd7-140">Here is an example of the response.</span></span> <span data-ttu-id="09dd7-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="09dd7-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T19:56:07Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
            "otherLabel": "Volunteer work",
            "type":"other",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="09dd7-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="09dd7-142">See also</span></span>

- [<span data-ttu-id="09dd7-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="09dd7-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="09dd7-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="09dd7-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


