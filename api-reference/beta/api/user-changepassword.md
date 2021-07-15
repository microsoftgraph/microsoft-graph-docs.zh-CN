---
title: user： changePassword
description: 更新自己的密码。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 7787ad62106cd5404bb0d5075d3d48d0ec1d6371
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442816"
---
# <a name="user-changepassword"></a><span data-ttu-id="79ef0-103">user： changePassword</span><span class="sxs-lookup"><span data-stu-id="79ef0-103">user: changePassword</span></span>

<span data-ttu-id="79ef0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ef0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79ef0-105">允许用户更新其密码。</span><span class="sxs-lookup"><span data-stu-id="79ef0-105">Enable the user to update their password.</span></span> <span data-ttu-id="79ef0-106">任何用户都可以更新其密码，而不属于任何管理员角色。</span><span class="sxs-lookup"><span data-stu-id="79ef0-106">Any user can update their password without belonging to any administrator role.</span></span>

## <a name="permissions"></a><span data-ttu-id="79ef0-107">权限</span><span class="sxs-lookup"><span data-stu-id="79ef0-107">Permissions</span></span>
<span data-ttu-id="79ef0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79ef0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="79ef0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79ef0-110">Permission type</span></span>      | <span data-ttu-id="79ef0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79ef0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79ef0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79ef0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79ef0-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79ef0-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79ef0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79ef0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79ef0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79ef0-115">Not supported.</span></span>    |
|<span data-ttu-id="79ef0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79ef0-116">Application</span></span> | <span data-ttu-id="79ef0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79ef0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79ef0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79ef0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/changePassword
```
## <a name="request-headers"></a><span data-ttu-id="79ef0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="79ef0-119">Request headers</span></span>
| <span data-ttu-id="79ef0-120">标头</span><span class="sxs-lookup"><span data-stu-id="79ef0-120">Header</span></span>       | <span data-ttu-id="79ef0-121">值</span><span class="sxs-lookup"><span data-stu-id="79ef0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79ef0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ef0-122">Authorization</span></span>  | <span data-ttu-id="79ef0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79ef0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79ef0-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="79ef0-125">Content-type</span></span>  | <span data-ttu-id="79ef0-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="79ef0-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79ef0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="79ef0-128">Request body</span></span>
<span data-ttu-id="79ef0-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="79ef0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79ef0-130">参数</span><span class="sxs-lookup"><span data-stu-id="79ef0-130">Parameter</span></span>    | <span data-ttu-id="79ef0-131">类型</span><span class="sxs-lookup"><span data-stu-id="79ef0-131">Type</span></span>   |<span data-ttu-id="79ef0-132">说明</span><span class="sxs-lookup"><span data-stu-id="79ef0-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79ef0-133">currentPassword</span><span class="sxs-lookup"><span data-stu-id="79ef0-133">currentPassword</span></span> | <span data-ttu-id="79ef0-134">String</span><span class="sxs-lookup"><span data-stu-id="79ef0-134">String</span></span> | <span data-ttu-id="79ef0-135">当前密码。</span><span class="sxs-lookup"><span data-stu-id="79ef0-135">Your current password.</span></span>|
| <span data-ttu-id="79ef0-136">newPassword</span><span class="sxs-lookup"><span data-stu-id="79ef0-136">newPassword</span></span> | <span data-ttu-id="79ef0-137">String</span><span class="sxs-lookup"><span data-stu-id="79ef0-137">String</span></span> | <span data-ttu-id="79ef0-138">新密码。</span><span class="sxs-lookup"><span data-stu-id="79ef0-138">Your new password.</span></span>|

## <a name="response"></a><span data-ttu-id="79ef0-139">响应</span><span class="sxs-lookup"><span data-stu-id="79ef0-139">Response</span></span>

<span data-ttu-id="79ef0-140">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="79ef0-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79ef0-141">示例</span><span class="sxs-lookup"><span data-stu-id="79ef0-141">Example</span></span>
<span data-ttu-id="79ef0-142">以下示例显示更新您自己的密码的请求。</span><span class="sxs-lookup"><span data-stu-id="79ef0-142">The following example shows a request to update your own password.</span></span>

### <a name="request"></a><span data-ttu-id="79ef0-143">请求</span><span class="sxs-lookup"><span data-stu-id="79ef0-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="79ef0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="79ef0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_changepassword"
}-->
```http
POST https://graph.microsoft.com/beta/me/changePassword
Content-type: application/json

{
    "currentPassword": "xWwvJ]6NMw+bWH-d",
    "newPassword": "0eM85N54wFxWwvJ]"
}
```
# <a name="c"></a>[<span data-ttu-id="79ef0-145">C#</span><span class="sxs-lookup"><span data-stu-id="79ef0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-changepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79ef0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79ef0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-changepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79ef0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79ef0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-changepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79ef0-148">Java</span><span class="sxs-lookup"><span data-stu-id="79ef0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-changepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="79ef0-149">响应</span><span class="sxs-lookup"><span data-stu-id="79ef0-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="79ef0-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="79ef0-150">See also</span></span>
+ [<span data-ttu-id="79ef0-151">更新用户的 passwordProfile 以重置其密码</span><span class="sxs-lookup"><span data-stu-id="79ef0-151">Update the passwordProfile of a user to reset their password</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)

<!-- uuid: a7c9a0de-8324-4f80-8d88-2e6d5838f3be
2021-06-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: changePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


