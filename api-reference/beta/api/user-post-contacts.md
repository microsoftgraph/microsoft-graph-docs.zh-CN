---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef5aa221d60d2a889b393cc9128de721e812066d
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637113"
---
# <a name="create-contact"></a><span data-ttu-id="4eb51-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="4eb51-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb51-104">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="4eb51-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4eb51-105">权限</span><span class="sxs-lookup"><span data-stu-id="4eb51-105">Permissions</span></span>
<span data-ttu-id="4eb51-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4eb51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb51-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4eb51-108">Permission type</span></span>      | <span data-ttu-id="4eb51-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4eb51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eb51-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4eb51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4eb51-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb51-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4eb51-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4eb51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb51-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb51-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4eb51-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4eb51-114">Application</span></span> | <span data-ttu-id="4eb51-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eb51-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eb51-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4eb51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="4eb51-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4eb51-117">Request headers</span></span>
| <span data-ttu-id="4eb51-118">标头</span><span class="sxs-lookup"><span data-stu-id="4eb51-118">Header</span></span>       | <span data-ttu-id="4eb51-119">值</span><span class="sxs-lookup"><span data-stu-id="4eb51-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4eb51-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eb51-120">Authorization</span></span>  | <span data-ttu-id="4eb51-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4eb51-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4eb51-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4eb51-123">Content-Type</span></span>  | <span data-ttu-id="4eb51-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb51-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4eb51-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4eb51-125">Request body</span></span>
<span data-ttu-id="4eb51-126">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eb51-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4eb51-127">响应</span><span class="sxs-lookup"><span data-stu-id="4eb51-127">Response</span></span>

<span data-ttu-id="4eb51-128">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[contact](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4eb51-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb51-129">示例</span><span class="sxs-lookup"><span data-stu-id="4eb51-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eb51-130">请求</span><span class="sxs-lookup"><span data-stu-id="4eb51-130">Request</span></span>
<span data-ttu-id="4eb51-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4eb51-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="4eb51-132">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eb51-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="4eb51-133">响应</span><span class="sxs-lookup"><span data-stu-id="4eb51-133">Response</span></span>
<span data-ttu-id="4eb51-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4eb51-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4eb51-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4eb51-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4eb51-138">语言</span><span class="sxs-lookup"><span data-stu-id="4eb51-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4eb51-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4eb51-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="4eb51-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4eb51-140">See also</span></span>

- [<span data-ttu-id="4eb51-141">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="4eb51-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4eb51-142">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="4eb51-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
