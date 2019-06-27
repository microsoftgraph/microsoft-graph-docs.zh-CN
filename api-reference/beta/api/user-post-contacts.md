---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fabcaa698c21b4a0118ca108861ffde4b751374a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269956"
---
# <a name="create-contact"></a><span data-ttu-id="0a099-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="0a099-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a099-104">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="0a099-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a099-105">权限</span><span class="sxs-lookup"><span data-stu-id="0a099-105">Permissions</span></span>
<span data-ttu-id="0a099-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a099-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a099-108">Permission type</span></span>      | <span data-ttu-id="0a099-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a099-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a099-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a099-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a099-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a099-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0a099-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a099-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a099-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a099-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0a099-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a099-114">Application</span></span> | <span data-ttu-id="0a099-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a099-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a099-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a099-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="0a099-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a099-117">Request headers</span></span>
| <span data-ttu-id="0a099-118">标头</span><span class="sxs-lookup"><span data-stu-id="0a099-118">Header</span></span>       | <span data-ttu-id="0a099-119">值</span><span class="sxs-lookup"><span data-stu-id="0a099-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a099-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a099-120">Authorization</span></span>  | <span data-ttu-id="0a099-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a099-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a099-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a099-123">Content-Type</span></span>  | <span data-ttu-id="0a099-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a099-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a099-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a099-125">Request body</span></span>
<span data-ttu-id="0a099-126">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a099-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0a099-127">响应</span><span class="sxs-lookup"><span data-stu-id="0a099-127">Response</span></span>

<span data-ttu-id="0a099-128">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[contact](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0a099-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a099-129">示例</span><span class="sxs-lookup"><span data-stu-id="0a099-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a099-130">请求</span><span class="sxs-lookup"><span data-stu-id="0a099-130">Request</span></span>
<span data-ttu-id="0a099-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a099-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="0a099-132">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a099-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0a099-133">响应</span><span class="sxs-lookup"><span data-stu-id="0a099-133">Response</span></span>
<span data-ttu-id="0a099-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a099-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a099-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0a099-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a099-138">C#</span><span class="sxs-lookup"><span data-stu-id="0a099-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a099-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a099-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0a099-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="0a099-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="0a099-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0a099-141">See also</span></span>

- [<span data-ttu-id="0a099-142">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0a099-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0a099-143">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="0a099-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
