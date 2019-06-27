---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 213d60a3dacb976d1bcc06509982ffe5a38a6359
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273890"
---
# <a name="create-contact"></a><span data-ttu-id="aaf72-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="aaf72-103">Create contact</span></span>

<span data-ttu-id="aaf72-104">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="aaf72-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaf72-105">权限</span><span class="sxs-lookup"><span data-stu-id="aaf72-105">Permissions</span></span>

<span data-ttu-id="aaf72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaf72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf72-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaf72-108">Permission type</span></span>      | <span data-ttu-id="aaf72-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aaf72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaf72-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aaf72-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaf72-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="aaf72-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaf72-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaf72-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="aaf72-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaf72-114">Application</span></span> | <span data-ttu-id="aaf72-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaf72-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaf72-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaf72-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="aaf72-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="aaf72-117">Request headers</span></span>

| <span data-ttu-id="aaf72-118">标头</span><span class="sxs-lookup"><span data-stu-id="aaf72-118">Header</span></span>       | <span data-ttu-id="aaf72-119">值</span><span class="sxs-lookup"><span data-stu-id="aaf72-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aaf72-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf72-120">Authorization</span></span>  | <span data-ttu-id="aaf72-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aaf72-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aaf72-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aaf72-123">Content-Type</span></span>  | <span data-ttu-id="aaf72-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="aaf72-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aaf72-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaf72-126">Request body</span></span>
<span data-ttu-id="aaf72-127">在请求正文中，提供 JSON 表示形式的 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaf72-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aaf72-128">响应</span><span class="sxs-lookup"><span data-stu-id="aaf72-128">Response</span></span>

<span data-ttu-id="aaf72-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaf72-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf72-130">示例</span><span class="sxs-lookup"><span data-stu-id="aaf72-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaf72-131">请求</span><span class="sxs-lookup"><span data-stu-id="aaf72-131">Request</span></span>

<span data-ttu-id="aaf72-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aaf72-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<span data-ttu-id="aaf72-133">在请求正文中，提供 JSON 表示形式的 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaf72-133">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="aaf72-134">响应</span><span class="sxs-lookup"><span data-stu-id="aaf72-134">Response</span></span>

<span data-ttu-id="aaf72-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aaf72-135">Here is an example of the response.</span></span> <span data-ttu-id="aaf72-136">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aaf72-136">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aaf72-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aaf72-137">All the properties will be returned from an actual call.</span></span>

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
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aaf72-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="aaf72-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aaf72-139">C#</span><span class="sxs-lookup"><span data-stu-id="aaf72-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aaf72-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="aaf72-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aaf72-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="aaf72-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
