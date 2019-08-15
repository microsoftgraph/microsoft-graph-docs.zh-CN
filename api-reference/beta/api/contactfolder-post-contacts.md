---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e61bfe311028fd303faa0dfbc71dcd6471879b9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417951"
---
# <a name="create-contact"></a><span data-ttu-id="fb85d-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="fb85d-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb85d-104">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="fb85d-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb85d-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb85d-105">Permissions</span></span>
<span data-ttu-id="fb85d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb85d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb85d-108">Permission type</span></span>      | <span data-ttu-id="fb85d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb85d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb85d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb85d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb85d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb85d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fb85d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb85d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb85d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb85d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fb85d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb85d-114">Application</span></span> | <span data-ttu-id="fb85d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb85d-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb85d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb85d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="fb85d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb85d-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="fb85d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb85d-118">Request headers</span></span>
| <span data-ttu-id="fb85d-119">标头</span><span class="sxs-lookup"><span data-stu-id="fb85d-119">Header</span></span>       | <span data-ttu-id="fb85d-120">值</span><span class="sxs-lookup"><span data-stu-id="fb85d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb85d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb85d-121">Authorization</span></span>  | <span data-ttu-id="fb85d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb85d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fb85d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb85d-124">Content-Type</span></span>  | <span data-ttu-id="fb85d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fb85d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb85d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb85d-127">Request body</span></span>
<span data-ttu-id="fb85d-128">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb85d-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fb85d-129">响应</span><span class="sxs-lookup"><span data-stu-id="fb85d-129">Response</span></span>

<span data-ttu-id="fb85d-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb85d-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb85d-131">示例</span><span class="sxs-lookup"><span data-stu-id="fb85d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb85d-132">请求</span><span class="sxs-lookup"><span data-stu-id="fb85d-132">Request</span></span>
<span data-ttu-id="fb85d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb85d-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb85d-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fb85d-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb85d-135">C#</span><span class="sxs-lookup"><span data-stu-id="fb85d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb85d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb85d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb85d-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="fb85d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fb85d-138">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb85d-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fb85d-139">响应</span><span class="sxs-lookup"><span data-stu-id="fb85d-139">Response</span></span>
<span data-ttu-id="fb85d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb85d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
