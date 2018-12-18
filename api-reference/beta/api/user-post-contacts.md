---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: dkershaw10
ms.openlocfilehash: cb95f9affa637dfb04109fc7192c6ddafe61362a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318989"
---
# <a name="create-contact"></a><span data-ttu-id="1b156-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="1b156-103">Create Contact</span></span>

> <span data-ttu-id="1b156-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b156-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b156-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b156-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b156-106">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="1b156-106">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b156-107">权限</span><span class="sxs-lookup"><span data-stu-id="1b156-107">Permissions</span></span>
<span data-ttu-id="1b156-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b156-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b156-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b156-110">Permission type</span></span>      | <span data-ttu-id="1b156-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b156-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b156-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b156-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b156-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b156-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b156-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b156-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b156-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b156-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b156-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b156-116">Application</span></span> | <span data-ttu-id="1b156-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b156-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b156-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b156-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="1b156-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b156-119">Request headers</span></span>
| <span data-ttu-id="1b156-120">标头</span><span class="sxs-lookup"><span data-stu-id="1b156-120">Header</span></span>       | <span data-ttu-id="1b156-121">值</span><span class="sxs-lookup"><span data-stu-id="1b156-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b156-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b156-122">Authorization</span></span>  | <span data-ttu-id="1b156-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b156-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b156-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b156-125">Content-Type</span></span>  | <span data-ttu-id="1b156-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b156-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b156-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b156-127">Request body</span></span>
<span data-ttu-id="1b156-128">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b156-128">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b156-129">响应</span><span class="sxs-lookup"><span data-stu-id="1b156-129">Response</span></span>

<span data-ttu-id="1b156-130">如果成功，此方法返回`201 Created`响应正文中的响应代码和[联系](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b156-130">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b156-131">示例</span><span class="sxs-lookup"><span data-stu-id="1b156-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b156-132">请求</span><span class="sxs-lookup"><span data-stu-id="1b156-132">Request</span></span>
<span data-ttu-id="1b156-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b156-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="1b156-134">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b156-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="1b156-135">响应</span><span class="sxs-lookup"><span data-stu-id="1b156-135">Response</span></span>
<span data-ttu-id="1b156-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b156-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1b156-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1b156-139">See also</span></span>

- [<span data-ttu-id="1b156-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="1b156-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1b156-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="1b156-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
