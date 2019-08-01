---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 85ec6d704402e1596a5376ed76fea155e61f4fe2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003124"
---
# <a name="create-contact"></a><span data-ttu-id="e0c15-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="e0c15-103">Create contact</span></span>

<span data-ttu-id="e0c15-104">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="e0c15-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0c15-105">权限</span><span class="sxs-lookup"><span data-stu-id="e0c15-105">Permissions</span></span>

<span data-ttu-id="e0c15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c15-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0c15-108">Permission type</span></span>      | <span data-ttu-id="e0c15-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0c15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0c15-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0c15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0c15-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0c15-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e0c15-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0c15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0c15-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0c15-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e0c15-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0c15-114">Application</span></span> | <span data-ttu-id="e0c15-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0c15-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0c15-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0c15-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="e0c15-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0c15-117">Request headers</span></span>

| <span data-ttu-id="e0c15-118">标头</span><span class="sxs-lookup"><span data-stu-id="e0c15-118">Header</span></span>       | <span data-ttu-id="e0c15-119">值</span><span class="sxs-lookup"><span data-stu-id="e0c15-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0c15-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0c15-120">Authorization</span></span>  | <span data-ttu-id="e0c15-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0c15-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0c15-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0c15-123">Content-Type</span></span>  | <span data-ttu-id="e0c15-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e0c15-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0c15-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0c15-126">Request body</span></span>
<span data-ttu-id="e0c15-127">在请求正文中，提供 JSON 表示形式的 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0c15-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0c15-128">响应</span><span class="sxs-lookup"><span data-stu-id="e0c15-128">Response</span></span>

<span data-ttu-id="e0c15-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0c15-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c15-130">示例</span><span class="sxs-lookup"><span data-stu-id="e0c15-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0c15-131">请求</span><span class="sxs-lookup"><span data-stu-id="e0c15-131">Request</span></span>

<span data-ttu-id="e0c15-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0c15-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e0c15-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e0c15-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0c15-134">C#</span><span class="sxs-lookup"><span data-stu-id="e0c15-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0c15-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0c15-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0c15-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="e0c15-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e0c15-137">Java</span><span class="sxs-lookup"><span data-stu-id="e0c15-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="e0c15-138">在请求正文中，提供 JSON 表示形式的 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0c15-138">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="e0c15-139">响应</span><span class="sxs-lookup"><span data-stu-id="e0c15-139">Response</span></span>

<span data-ttu-id="e0c15-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0c15-140">Here is an example of the response.</span></span> <span data-ttu-id="e0c15-141">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0c15-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e0c15-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0c15-142">All the properties will be returned from an actual call.</span></span>

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
  ]
}-->
