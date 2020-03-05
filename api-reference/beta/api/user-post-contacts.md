---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d86f100f3343ffba2b3302927129bdd7a575329
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451705"
---
# <a name="create-contact"></a><span data-ttu-id="82ba5-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="82ba5-103">Create Contact</span></span>

<span data-ttu-id="82ba5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82ba5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82ba5-105">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="82ba5-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="82ba5-106">权限</span><span class="sxs-lookup"><span data-stu-id="82ba5-106">Permissions</span></span>
<span data-ttu-id="82ba5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82ba5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82ba5-109">Permission type</span></span>      | <span data-ttu-id="82ba5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82ba5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82ba5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82ba5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="82ba5-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82ba5-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="82ba5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82ba5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82ba5-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82ba5-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="82ba5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82ba5-115">Application</span></span> | <span data-ttu-id="82ba5-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82ba5-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="82ba5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82ba5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="82ba5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="82ba5-118">Request headers</span></span>
| <span data-ttu-id="82ba5-119">标头</span><span class="sxs-lookup"><span data-stu-id="82ba5-119">Header</span></span>       | <span data-ttu-id="82ba5-120">值</span><span class="sxs-lookup"><span data-stu-id="82ba5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82ba5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82ba5-121">Authorization</span></span>  | <span data-ttu-id="82ba5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82ba5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82ba5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82ba5-124">Content-Type</span></span>  | <span data-ttu-id="82ba5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82ba5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82ba5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82ba5-126">Request body</span></span>
<span data-ttu-id="82ba5-127">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82ba5-127">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="82ba5-128">响应</span><span class="sxs-lookup"><span data-stu-id="82ba5-128">Response</span></span>

<span data-ttu-id="82ba5-129">如果成功，此方法在`201 Created`响应正文中返回响应代码和[contact](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82ba5-129">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82ba5-130">示例</span><span class="sxs-lookup"><span data-stu-id="82ba5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82ba5-131">请求</span><span class="sxs-lookup"><span data-stu-id="82ba5-131">Request</span></span>
<span data-ttu-id="82ba5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82ba5-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82ba5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="82ba5-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82ba5-134">C#</span><span class="sxs-lookup"><span data-stu-id="82ba5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82ba5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82ba5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82ba5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82ba5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="82ba5-137">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82ba5-137">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="82ba5-138">响应</span><span class="sxs-lookup"><span data-stu-id="82ba5-138">Response</span></span>
<span data-ttu-id="82ba5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82ba5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="82ba5-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82ba5-142">See also</span></span>

- [<span data-ttu-id="82ba5-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="82ba5-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="82ba5-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="82ba5-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
