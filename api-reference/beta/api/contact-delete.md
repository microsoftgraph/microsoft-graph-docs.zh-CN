---
title: 删除联系人
description: 删除联系人。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9f3e0a56d3c9f4b1a1858dc350e264eb18a11056
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591741"
---
# <a name="delete-contact"></a><span data-ttu-id="c7471-103">删除联系人</span><span class="sxs-lookup"><span data-stu-id="c7471-103">Delete contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7471-104">删除联系人。</span><span class="sxs-lookup"><span data-stu-id="c7471-104">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7471-105">权限</span><span class="sxs-lookup"><span data-stu-id="c7471-105">Permissions</span></span>
<span data-ttu-id="c7471-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7471-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7471-108">Permission type</span></span>      | <span data-ttu-id="c7471-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7471-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7471-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7471-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7471-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7471-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c7471-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7471-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7471-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7471-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c7471-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7471-114">Application</span></span> | <span data-ttu-id="c7471-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7471-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7471-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7471-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c7471-117">用户的默认[contactFolder](../resources/contactfolder.md)中的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="c7471-117">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="c7471-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="c7471-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="c7471-119">[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="c7471-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="c7471-120">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="c7471-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c7471-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7471-121">Request headers</span></span>
| <span data-ttu-id="c7471-122">标头</span><span class="sxs-lookup"><span data-stu-id="c7471-122">Header</span></span>       | <span data-ttu-id="c7471-123">值</span><span class="sxs-lookup"><span data-stu-id="c7471-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7471-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7471-124">Authorization</span></span>  | <span data-ttu-id="c7471-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7471-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7471-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7471-127">Request body</span></span>
<span data-ttu-id="c7471-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7471-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7471-129">响应</span><span class="sxs-lookup"><span data-stu-id="c7471-129">Response</span></span>

<span data-ttu-id="c7471-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c7471-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7471-132">示例</span><span class="sxs-lookup"><span data-stu-id="c7471-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7471-133">请求</span><span class="sxs-lookup"><span data-stu-id="c7471-133">Request</span></span>
<span data-ttu-id="c7471-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7471-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="c7471-135">响应</span><span class="sxs-lookup"><span data-stu-id="c7471-135">Response</span></span>
<span data-ttu-id="c7471-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7471-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c7471-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c7471-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c7471-140">语言</span><span class="sxs-lookup"><span data-stu-id="c7471-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7471-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7471-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
