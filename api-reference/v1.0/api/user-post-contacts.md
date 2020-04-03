---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 497206bd7174aa9fd7d32bd574366ca9e1bb44e3
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109010"
---
# <a name="create-contact"></a><span data-ttu-id="67ce9-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="67ce9-103">Create Contact</span></span>

<span data-ttu-id="67ce9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67ce9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67ce9-105">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人终结点中。</span><span class="sxs-lookup"><span data-stu-id="67ce9-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="67ce9-106">权限</span><span class="sxs-lookup"><span data-stu-id="67ce9-106">Permissions</span></span>
<span data-ttu-id="67ce9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67ce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ce9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67ce9-109">Permission type</span></span>      | <span data-ttu-id="67ce9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67ce9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67ce9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67ce9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67ce9-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67ce9-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="67ce9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67ce9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ce9-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67ce9-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="67ce9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="67ce9-115">Application</span></span> | <span data-ttu-id="67ce9-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67ce9-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="67ce9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67ce9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="67ce9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="67ce9-118">Request headers</span></span>
| <span data-ttu-id="67ce9-119">标头</span><span class="sxs-lookup"><span data-stu-id="67ce9-119">Header</span></span>       | <span data-ttu-id="67ce9-120">值</span><span class="sxs-lookup"><span data-stu-id="67ce9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67ce9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67ce9-121">Authorization</span></span>  | <span data-ttu-id="67ce9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67ce9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="67ce9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67ce9-124">Content-Type</span></span>  | <span data-ttu-id="67ce9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67ce9-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67ce9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67ce9-126">Request body</span></span>
<span data-ttu-id="67ce9-127">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67ce9-127">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="67ce9-128">响应</span><span class="sxs-lookup"><span data-stu-id="67ce9-128">Response</span></span>

<span data-ttu-id="67ce9-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67ce9-129">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67ce9-130">示例</span><span class="sxs-lookup"><span data-stu-id="67ce9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67ce9-131">请求</span><span class="sxs-lookup"><span data-stu-id="67ce9-131">Request</span></span>
<span data-ttu-id="67ce9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67ce9-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67ce9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ce9-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67ce9-134">C#</span><span class="sxs-lookup"><span data-stu-id="67ce9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67ce9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ce9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67ce9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ce9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67ce9-137">Java</span><span class="sxs-lookup"><span data-stu-id="67ce9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="67ce9-138">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67ce9-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="67ce9-139">响应</span><span class="sxs-lookup"><span data-stu-id="67ce9-139">Response</span></span>
<span data-ttu-id="67ce9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67ce9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
