---
title: 删除联系人
description: 删除联系人。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3235e460c43aa2c4062ffbbbcb798d2e6a6043fe
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277523"
---
# <a name="delete-contact"></a><span data-ttu-id="562cb-103">删除联系人</span><span class="sxs-lookup"><span data-stu-id="562cb-103">Delete contact</span></span>

<span data-ttu-id="562cb-104">删除联系人。</span><span class="sxs-lookup"><span data-stu-id="562cb-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="562cb-105">权限</span><span class="sxs-lookup"><span data-stu-id="562cb-105">Permissions</span></span>
<span data-ttu-id="562cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="562cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="562cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="562cb-108">Permission type</span></span>      | <span data-ttu-id="562cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="562cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="562cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="562cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="562cb-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="562cb-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="562cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="562cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="562cb-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="562cb-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="562cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="562cb-114">Application</span></span> | <span data-ttu-id="562cb-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="562cb-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="562cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="562cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="562cb-117">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="562cb-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="562cb-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="562cb-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="562cb-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="562cb-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="562cb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="562cb-121">Request headers</span></span>
| <span data-ttu-id="562cb-122">标头</span><span class="sxs-lookup"><span data-stu-id="562cb-122">Header</span></span>       | <span data-ttu-id="562cb-123">值</span><span class="sxs-lookup"><span data-stu-id="562cb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="562cb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="562cb-124">Authorization</span></span>  | <span data-ttu-id="562cb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="562cb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="562cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="562cb-127">Request body</span></span>
<span data-ttu-id="562cb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="562cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="562cb-129">响应</span><span class="sxs-lookup"><span data-stu-id="562cb-129">Response</span></span>

<span data-ttu-id="562cb-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="562cb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="562cb-132">示例</span><span class="sxs-lookup"><span data-stu-id="562cb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="562cb-133">请求</span><span class="sxs-lookup"><span data-stu-id="562cb-133">Request</span></span>
<span data-ttu-id="562cb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="562cb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="562cb-135">响应</span><span class="sxs-lookup"><span data-stu-id="562cb-135">Response</span></span>
<span data-ttu-id="562cb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="562cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="562cb-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="562cb-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="562cb-140">C#</span><span class="sxs-lookup"><span data-stu-id="562cb-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="562cb-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="562cb-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="562cb-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="562cb-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_contact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
