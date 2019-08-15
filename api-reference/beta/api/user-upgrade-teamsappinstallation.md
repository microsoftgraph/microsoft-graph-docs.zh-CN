---
title: 'teamsAppInstallation: upgrade'
description: 在用户的个人作用域中升级应用程序安装
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ed1e1a2a43499fd1634c62abfe830167d32a2e03
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421769"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="74e01-103">teamsAppInstallation: upgrade</span><span class="sxs-lookup"><span data-stu-id="74e01-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74e01-104">将指定[用户](../resources/user.md)的个人作用域中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="74e01-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e01-105">权限</span><span class="sxs-lookup"><span data-stu-id="74e01-105">Permissions</span></span>

<span data-ttu-id="74e01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e01-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="74e01-108">Permission type</span></span>      | <span data-ttu-id="74e01-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74e01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e01-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74e01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74e01-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e01-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="74e01-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74e01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e01-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e01-113">Not supported.</span></span>    |
|<span data-ttu-id="74e01-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="74e01-114">Application</span></span> | <span data-ttu-id="74e01-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e01-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e01-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74e01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="74e01-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="74e01-117">Request headers</span></span>

| <span data-ttu-id="74e01-118">标头</span><span class="sxs-lookup"><span data-stu-id="74e01-118">Header</span></span>       | <span data-ttu-id="74e01-119">值</span><span class="sxs-lookup"><span data-stu-id="74e01-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74e01-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e01-120">Authorization</span></span>  | <span data-ttu-id="74e01-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74e01-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74e01-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="74e01-123">Request body</span></span>

<span data-ttu-id="74e01-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74e01-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74e01-125">响应</span><span class="sxs-lookup"><span data-stu-id="74e01-125">Response</span></span>

<span data-ttu-id="74e01-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="74e01-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e01-128">示例</span><span class="sxs-lookup"><span data-stu-id="74e01-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="74e01-129">请求</span><span class="sxs-lookup"><span data-stu-id="74e01-129">Request</span></span>

<span data-ttu-id="74e01-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74e01-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="74e01-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="74e01-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74e01-132">C#</span><span class="sxs-lookup"><span data-stu-id="74e01-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74e01-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74e01-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74e01-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="74e01-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74e01-135">响应</span><span class="sxs-lookup"><span data-stu-id="74e01-135">Response</span></span>

<span data-ttu-id="74e01-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74e01-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
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
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
