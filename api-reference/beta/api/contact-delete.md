---
title: 删除联系人
description: 删除联系人。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 909e0d8e3b0e3e811035db29c071c476b562487a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382082"
---
# <a name="delete-contact"></a><span data-ttu-id="0d83f-103">删除联系人</span><span class="sxs-lookup"><span data-stu-id="0d83f-103">Delete contact</span></span>

<span data-ttu-id="0d83f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d83f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d83f-105">删除联系人。</span><span class="sxs-lookup"><span data-stu-id="0d83f-105">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d83f-106">权限</span><span class="sxs-lookup"><span data-stu-id="0d83f-106">Permissions</span></span>
<span data-ttu-id="0d83f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d83f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d83f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d83f-109">Permission type</span></span>      | <span data-ttu-id="0d83f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d83f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d83f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d83f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d83f-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d83f-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d83f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d83f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d83f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d83f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d83f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d83f-115">Application</span></span> | <span data-ttu-id="0d83f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d83f-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d83f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d83f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0d83f-118">用户的默认[contactFolder](../resources/contactfolder.md)中的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0d83f-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="0d83f-119">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0d83f-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="0d83f-120">[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="0d83f-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="0d83f-121">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="0d83f-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0d83f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d83f-122">Request headers</span></span>
| <span data-ttu-id="0d83f-123">标头</span><span class="sxs-lookup"><span data-stu-id="0d83f-123">Header</span></span>       | <span data-ttu-id="0d83f-124">值</span><span class="sxs-lookup"><span data-stu-id="0d83f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d83f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d83f-125">Authorization</span></span>  | <span data-ttu-id="0d83f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d83f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d83f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d83f-128">Request body</span></span>
<span data-ttu-id="0d83f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d83f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d83f-130">响应</span><span class="sxs-lookup"><span data-stu-id="0d83f-130">Response</span></span>

<span data-ttu-id="0d83f-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0d83f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d83f-133">示例</span><span class="sxs-lookup"><span data-stu-id="0d83f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d83f-134">请求</span><span class="sxs-lookup"><span data-stu-id="0d83f-134">Request</span></span>
<span data-ttu-id="0d83f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d83f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d83f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d83f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="0d83f-137">C#</span><span class="sxs-lookup"><span data-stu-id="0d83f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d83f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d83f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d83f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d83f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0d83f-140">响应</span><span class="sxs-lookup"><span data-stu-id="0d83f-140">Response</span></span>
<span data-ttu-id="0d83f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d83f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
