---
title: 删除联系人
description: 删除联系人。
ms.openlocfilehash: fec4ec30430114f023577043b0351683fc25189e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042902"
---
# <a name="delete-contact"></a><span data-ttu-id="6b75f-103">删除联系人</span><span class="sxs-lookup"><span data-stu-id="6b75f-103">Delete contact</span></span>

> <span data-ttu-id="6b75f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6b75f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b75f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b75f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b75f-106">删除联系人。</span><span class="sxs-lookup"><span data-stu-id="6b75f-106">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b75f-107">权限</span><span class="sxs-lookup"><span data-stu-id="6b75f-107">Permissions</span></span>
<span data-ttu-id="6b75f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b75f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b75f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b75f-110">Permission type</span></span>      | <span data-ttu-id="6b75f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b75f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b75f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b75f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6b75f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b75f-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6b75f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b75f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b75f-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b75f-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6b75f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b75f-116">Application</span></span> | <span data-ttu-id="6b75f-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b75f-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b75f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b75f-118">HTTP request</span></span>
<span data-ttu-id="6b75f-119"><!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)从用户的默认[contactFolder](../resources/contactfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="6b75f-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="6b75f-120">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="6b75f-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="6b75f-121">[联系人](../resources/contact.md) [contactFolder](../resources/mailfolder.md)子文件夹中包含。</span><span class="sxs-lookup"><span data-stu-id="6b75f-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="6b75f-122">下面的示例演示一个级别的嵌套，但联系人可以位于子级的子级，依此类推。</span><span class="sxs-lookup"><span data-stu-id="6b75f-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6b75f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b75f-123">Request headers</span></span>
| <span data-ttu-id="6b75f-124">标头</span><span class="sxs-lookup"><span data-stu-id="6b75f-124">Header</span></span>       | <span data-ttu-id="6b75f-125">值</span><span class="sxs-lookup"><span data-stu-id="6b75f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b75f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b75f-126">Authorization</span></span>  | <span data-ttu-id="6b75f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b75f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b75f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b75f-129">Request body</span></span>
<span data-ttu-id="6b75f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b75f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b75f-131">响应</span><span class="sxs-lookup"><span data-stu-id="6b75f-131">Response</span></span>

<span data-ttu-id="6b75f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6b75f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b75f-134">示例</span><span class="sxs-lookup"><span data-stu-id="6b75f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b75f-135">请求</span><span class="sxs-lookup"><span data-stu-id="6b75f-135">Request</span></span>
<span data-ttu-id="6b75f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b75f-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="6b75f-137">响应</span><span class="sxs-lookup"><span data-stu-id="6b75f-137">Response</span></span>
<span data-ttu-id="6b75f-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b75f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->