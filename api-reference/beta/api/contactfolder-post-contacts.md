---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 27e765335b2ae9c4e81668adfb090746773b4282
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047068"
---
# <a name="create-contact"></a><span data-ttu-id="0b9e5-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="0b9e5-103">Create Contact</span></span>

<span data-ttu-id="0b9e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b9e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b9e5-105">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b9e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="0b9e5-106">Permissions</span></span>
<span data-ttu-id="0b9e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b9e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b9e5-109">Permission type</span></span>      | <span data-ttu-id="0b9e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b9e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b9e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b9e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b9e5-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b9e5-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0b9e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b9e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b9e5-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b9e5-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0b9e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b9e5-115">Application</span></span> | <span data-ttu-id="0b9e5-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b9e5-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b9e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b9e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="0b9e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b9e5-118">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="0b9e5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b9e5-119">Request headers</span></span>
| <span data-ttu-id="0b9e5-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b9e5-120">Header</span></span>       | <span data-ttu-id="0b9e5-121">值</span><span class="sxs-lookup"><span data-stu-id="0b9e5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b9e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b9e5-122">Authorization</span></span>  | <span data-ttu-id="0b9e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0b9e5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b9e5-125">Content-Type</span></span>  | <span data-ttu-id="0b9e5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b9e5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b9e5-128">Request body</span></span>
<span data-ttu-id="0b9e5-129">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-129">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0b9e5-130">响应</span><span class="sxs-lookup"><span data-stu-id="0b9e5-130">Response</span></span>

<span data-ttu-id="0b9e5-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-131">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b9e5-132">示例</span><span class="sxs-lookup"><span data-stu-id="0b9e5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b9e5-133">请求</span><span class="sxs-lookup"><span data-stu-id="0b9e5-133">Request</span></span>
<span data-ttu-id="0b9e5-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b9e5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b9e5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="c"></a>[<span data-ttu-id="0b9e5-136">C#</span><span class="sxs-lookup"><span data-stu-id="0b9e5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b9e5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b9e5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b9e5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b9e5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b9e5-139">Java</span><span class="sxs-lookup"><span data-stu-id="0b9e5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0b9e5-140">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-140">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0b9e5-141">响应</span><span class="sxs-lookup"><span data-stu-id="0b9e5-141">Response</span></span>
<span data-ttu-id="0b9e5-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-142">Here is an example of the response.</span></span> <span data-ttu-id="0b9e5-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b9e5-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

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


