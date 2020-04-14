---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d0238dc7b065e7fd8be884c47cbcab8622df81bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43360978"
---
# <a name="create-contact"></a><span data-ttu-id="38c41-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="38c41-103">Create Contact</span></span>

<span data-ttu-id="38c41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38c41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38c41-105">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="38c41-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="38c41-106">权限</span><span class="sxs-lookup"><span data-stu-id="38c41-106">Permissions</span></span>
<span data-ttu-id="38c41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38c41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38c41-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="38c41-109">Permission type</span></span>      | <span data-ttu-id="38c41-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38c41-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38c41-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38c41-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38c41-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38c41-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="38c41-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38c41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38c41-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38c41-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="38c41-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="38c41-115">Application</span></span> | <span data-ttu-id="38c41-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38c41-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="38c41-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38c41-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="38c41-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="38c41-118">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="38c41-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38c41-119">Request headers</span></span>
| <span data-ttu-id="38c41-120">标头</span><span class="sxs-lookup"><span data-stu-id="38c41-120">Header</span></span>       | <span data-ttu-id="38c41-121">值</span><span class="sxs-lookup"><span data-stu-id="38c41-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38c41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38c41-122">Authorization</span></span>  | <span data-ttu-id="38c41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38c41-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="38c41-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38c41-125">Content-Type</span></span>  | <span data-ttu-id="38c41-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="38c41-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38c41-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="38c41-128">Request body</span></span>
<span data-ttu-id="38c41-129">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38c41-129">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="38c41-130">响应</span><span class="sxs-lookup"><span data-stu-id="38c41-130">Response</span></span>

<span data-ttu-id="38c41-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38c41-131">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38c41-132">示例</span><span class="sxs-lookup"><span data-stu-id="38c41-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38c41-133">请求</span><span class="sxs-lookup"><span data-stu-id="38c41-133">Request</span></span>
<span data-ttu-id="38c41-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38c41-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38c41-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="38c41-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="38c41-136">C#</span><span class="sxs-lookup"><span data-stu-id="38c41-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38c41-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38c41-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38c41-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38c41-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="38c41-139">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38c41-139">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="38c41-140">响应</span><span class="sxs-lookup"><span data-stu-id="38c41-140">Response</span></span>
<span data-ttu-id="38c41-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38c41-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
