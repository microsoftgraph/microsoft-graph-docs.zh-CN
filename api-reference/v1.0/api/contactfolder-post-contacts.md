---
title: 创建联系人
description: 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 78d967862d586c064975c82872b8263a92c345e5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467658"
---
# <a name="create-contact"></a><span data-ttu-id="ac976-103">创建联系人</span><span class="sxs-lookup"><span data-stu-id="ac976-103">Create contact</span></span>

<span data-ttu-id="ac976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac976-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac976-105">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="ac976-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac976-106">权限</span><span class="sxs-lookup"><span data-stu-id="ac976-106">Permissions</span></span>

<span data-ttu-id="ac976-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac976-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac976-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac976-109">Permission type</span></span>      | <span data-ttu-id="ac976-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac976-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac976-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac976-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ac976-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac976-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ac976-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac976-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac976-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac976-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ac976-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac976-115">Application</span></span> | <span data-ttu-id="ac976-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac976-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac976-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac976-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="ac976-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac976-118">Request headers</span></span>

| <span data-ttu-id="ac976-119">标头</span><span class="sxs-lookup"><span data-stu-id="ac976-119">Header</span></span>       | <span data-ttu-id="ac976-120">值</span><span class="sxs-lookup"><span data-stu-id="ac976-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac976-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac976-121">Authorization</span></span>  | <span data-ttu-id="ac976-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac976-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ac976-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac976-124">Content-Type</span></span>  | <span data-ttu-id="ac976-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ac976-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac976-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac976-127">Request body</span></span>
<span data-ttu-id="ac976-128">在请求正文中，提供 JSON 表示形式的 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac976-128">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ac976-129">响应</span><span class="sxs-lookup"><span data-stu-id="ac976-129">Response</span></span>

<span data-ttu-id="ac976-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac976-130">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac976-131">示例</span><span class="sxs-lookup"><span data-stu-id="ac976-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac976-132">请求</span><span class="sxs-lookup"><span data-stu-id="ac976-132">Request</span></span>

<span data-ttu-id="ac976-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac976-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac976-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac976-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac976-135">C#</span><span class="sxs-lookup"><span data-stu-id="ac976-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac976-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac976-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac976-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac976-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac976-138">Java</span><span class="sxs-lookup"><span data-stu-id="ac976-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="ac976-139">在请求正文中，提供 JSON 表示形式的 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac976-139">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="ac976-140">响应</span><span class="sxs-lookup"><span data-stu-id="ac976-140">Response</span></span>

<span data-ttu-id="ac976-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ac976-141">Here is an example of the response.</span></span> <span data-ttu-id="ac976-142">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac976-142">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ac976-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ac976-143">All the properties will be returned from an actual call.</span></span>

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
