---
title: 为用户安装应用程序
description: 在指定用户的个人作用域中安装应用程序。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ff8d17444cf3b488d5d849399b8032f9c0a1bc1e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409175"
---
# <a name="install-app-for-user"></a><span data-ttu-id="6cade-103">为用户安装应用程序</span><span class="sxs-lookup"><span data-stu-id="6cade-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cade-104">在指定[用户](../resources/user.md)的个人作用域中安装[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="6cade-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cade-105">权限</span><span class="sxs-lookup"><span data-stu-id="6cade-105">Permissions</span></span>

<span data-ttu-id="6cade-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cade-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cade-108">Permission type</span></span>      | <span data-ttu-id="6cade-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cade-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cade-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cade-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6cade-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cade-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="6cade-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cade-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cade-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cade-113">Not supported.</span></span>    |
|<span data-ttu-id="6cade-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cade-114">Application</span></span> | <span data-ttu-id="6cade-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cade-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cade-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cade-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="6cade-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cade-117">Request headers</span></span>

| <span data-ttu-id="6cade-118">标头</span><span class="sxs-lookup"><span data-stu-id="6cade-118">Header</span></span>       | <span data-ttu-id="6cade-119">值</span><span class="sxs-lookup"><span data-stu-id="6cade-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cade-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cade-120">Authorization</span></span>  | <span data-ttu-id="6cade-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cade-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cade-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cade-123">Request body</span></span>

<span data-ttu-id="6cade-124">请求正文应包含要添加的现有目录应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="6cade-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="6cade-125">属性</span><span class="sxs-lookup"><span data-stu-id="6cade-125">Property</span></span>   | <span data-ttu-id="6cade-126">类型</span><span class="sxs-lookup"><span data-stu-id="6cade-126">Type</span></span> |<span data-ttu-id="6cade-127">说明</span><span class="sxs-lookup"><span data-stu-id="6cade-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cade-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6cade-128">teamsApp</span></span>|<span data-ttu-id="6cade-129">String</span><span class="sxs-lookup"><span data-stu-id="6cade-129">String</span></span>|<span data-ttu-id="6cade-130">要添加的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="6cade-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="6cade-131">响应</span><span class="sxs-lookup"><span data-stu-id="6cade-131">Response</span></span>

<span data-ttu-id="6cade-p103">如果成功，此方法返回 `201 Created` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6cade-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cade-134">示例</span><span class="sxs-lookup"><span data-stu-id="6cade-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cade-135">请求</span><span class="sxs-lookup"><span data-stu-id="6cade-135">Request</span></span>

<span data-ttu-id="6cade-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6cade-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6cade-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6cade-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6cade-138">C#</span><span class="sxs-lookup"><span data-stu-id="6cade-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cade-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cade-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6cade-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="6cade-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6cade-141">响应</span><span class="sxs-lookup"><span data-stu-id="6cade-141">Response</span></span>

<span data-ttu-id="6cade-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6cade-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
