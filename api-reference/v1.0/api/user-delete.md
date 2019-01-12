---
title: 删除用户
description: 删除用户。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93097c1d2f3f88e3e1f6b4a0166883728b402ba4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987088"
---
# <a name="delete-a-user"></a><span data-ttu-id="ec586-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="ec586-103">Delete a user</span></span>

<span data-ttu-id="ec586-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="ec586-104">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec586-105">权限</span><span class="sxs-lookup"><span data-stu-id="ec586-105">Permissions</span></span>
<span data-ttu-id="ec586-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec586-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec586-108">Permission type</span></span>      | <span data-ttu-id="ec586-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec586-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec586-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec586-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec586-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec586-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec586-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec586-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec586-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec586-113">Not supported.</span></span>    |
|<span data-ttu-id="ec586-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec586-114">Application</span></span> | <span data-ttu-id="ec586-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec586-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec586-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec586-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="ec586-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec586-117">Request headers</span></span>
| <span data-ttu-id="ec586-118">标头</span><span class="sxs-lookup"><span data-stu-id="ec586-118">Header</span></span>       | <span data-ttu-id="ec586-119">值</span><span class="sxs-lookup"><span data-stu-id="ec586-119">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ec586-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec586-120">Authorization</span></span>  | <span data-ttu-id="ec586-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec586-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec586-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec586-123">Request body</span></span>
<span data-ttu-id="ec586-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec586-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec586-125">响应</span><span class="sxs-lookup"><span data-stu-id="ec586-125">Response</span></span>

<span data-ttu-id="ec586-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ec586-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec586-128">示例</span><span class="sxs-lookup"><span data-stu-id="ec586-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec586-129">请求</span><span class="sxs-lookup"><span data-stu-id="ec586-129">Request</span></span>
<span data-ttu-id="ec586-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec586-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="ec586-131">响应</span><span class="sxs-lookup"><span data-stu-id="ec586-131">Response</span></span>
<span data-ttu-id="ec586-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ec586-132">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
