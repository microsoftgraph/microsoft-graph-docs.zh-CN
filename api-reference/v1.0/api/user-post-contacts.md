---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab836089b926324b5163c12ab234f6bfc791abe8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086849"
---
# <a name="create-contact"></a><span data-ttu-id="d905b-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="d905b-103">Create Contact</span></span>

<span data-ttu-id="d905b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d905b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d905b-105">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="d905b-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d905b-106">权限</span><span class="sxs-lookup"><span data-stu-id="d905b-106">Permissions</span></span>
<span data-ttu-id="d905b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d905b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d905b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d905b-109">Permission type</span></span>      | <span data-ttu-id="d905b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d905b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d905b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d905b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d905b-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d905b-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d905b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d905b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d905b-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d905b-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d905b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d905b-115">Application</span></span> | <span data-ttu-id="d905b-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d905b-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d905b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d905b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="d905b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d905b-118">Request headers</span></span>
| <span data-ttu-id="d905b-119">标头</span><span class="sxs-lookup"><span data-stu-id="d905b-119">Header</span></span>       | <span data-ttu-id="d905b-120">值</span><span class="sxs-lookup"><span data-stu-id="d905b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d905b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d905b-121">Authorization</span></span>  | <span data-ttu-id="d905b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d905b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d905b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d905b-124">Content-Type</span></span>  | <span data-ttu-id="d905b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d905b-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d905b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d905b-126">Request body</span></span>
<span data-ttu-id="d905b-127">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d905b-127">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d905b-128">响应</span><span class="sxs-lookup"><span data-stu-id="d905b-128">Response</span></span>

<span data-ttu-id="d905b-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d905b-129">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d905b-130">示例</span><span class="sxs-lookup"><span data-stu-id="d905b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d905b-131">请求</span><span class="sxs-lookup"><span data-stu-id="d905b-131">Request</span></span>
<span data-ttu-id="d905b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d905b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d905b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d905b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d905b-134">C#</span><span class="sxs-lookup"><span data-stu-id="d905b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d905b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d905b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d905b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d905b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d905b-137">Java</span><span class="sxs-lookup"><span data-stu-id="d905b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d905b-138">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d905b-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d905b-139">响应</span><span class="sxs-lookup"><span data-stu-id="d905b-139">Response</span></span>
<span data-ttu-id="d905b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d905b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

