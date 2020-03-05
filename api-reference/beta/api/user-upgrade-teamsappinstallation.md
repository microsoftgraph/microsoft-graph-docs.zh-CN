---
title: teamsAppInstallation： upgrade
description: 在用户的个人作用域中升级应用程序安装
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 01a08e81279883225b2cf096e7f6b8767e8eb0d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451594"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="d84a9-103">teamsAppInstallation： upgrade</span><span class="sxs-lookup"><span data-stu-id="d84a9-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="d84a9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d84a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d84a9-105">将指定[用户](../resources/user.md)的个人作用域中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d84a9-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="d84a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d84a9-106">Permissions</span></span>

<span data-ttu-id="d84a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d84a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d84a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d84a9-109">Permission type</span></span>      | <span data-ttu-id="d84a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d84a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d84a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d84a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d84a9-112">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d84a9-112">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="d84a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d84a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d84a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d84a9-114">Not supported.</span></span>    |
|<span data-ttu-id="d84a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d84a9-115">Application</span></span> | <span data-ttu-id="d84a9-116">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d84a9-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d84a9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d84a9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="d84a9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d84a9-118">Request headers</span></span>

| <span data-ttu-id="d84a9-119">标头</span><span class="sxs-lookup"><span data-stu-id="d84a9-119">Header</span></span>       | <span data-ttu-id="d84a9-120">值</span><span class="sxs-lookup"><span data-stu-id="d84a9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d84a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d84a9-121">Authorization</span></span>  | <span data-ttu-id="d84a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d84a9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d84a9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d84a9-124">Request body</span></span>

<span data-ttu-id="d84a9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d84a9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d84a9-126">响应</span><span class="sxs-lookup"><span data-stu-id="d84a9-126">Response</span></span>

<span data-ttu-id="d84a9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d84a9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d84a9-129">示例</span><span class="sxs-lookup"><span data-stu-id="d84a9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d84a9-130">请求</span><span class="sxs-lookup"><span data-stu-id="d84a9-130">Request</span></span>

<span data-ttu-id="d84a9-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d84a9-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d84a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d84a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="d84a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="d84a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d84a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d84a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d84a9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d84a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d84a9-136">响应</span><span class="sxs-lookup"><span data-stu-id="d84a9-136">Response</span></span>

<span data-ttu-id="d84a9-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d84a9-137">The following is an example of the response.</span></span>

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
