---
title: 升级团队中的应用程序
description: 升级团队中的应用程序安装
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 69698bf588b6aec789720a7cc1d46a114a5e0621
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421300"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="8a323-103">升级团队中的应用程序</span><span class="sxs-lookup"><span data-stu-id="8a323-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a323-104">将[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a323-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a323-105">权限</span><span class="sxs-lookup"><span data-stu-id="8a323-105">Permissions</span></span>

<span data-ttu-id="8a323-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a323-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a323-108">Permission type</span></span>      | <span data-ttu-id="8a323-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a323-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a323-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a323-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a323-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a323-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a323-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a323-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a323-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a323-113">Not supported.</span></span>    |
|<span data-ttu-id="8a323-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a323-114">Application</span></span> | <span data-ttu-id="8a323-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a323-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a323-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a323-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="8a323-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a323-117">Request headers</span></span>

| <span data-ttu-id="8a323-118">标头</span><span class="sxs-lookup"><span data-stu-id="8a323-118">Header</span></span>       | <span data-ttu-id="8a323-119">值</span><span class="sxs-lookup"><span data-stu-id="8a323-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a323-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a323-120">Authorization</span></span>  | <span data-ttu-id="8a323-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a323-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a323-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a323-123">Request body</span></span>

<span data-ttu-id="8a323-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a323-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a323-125">响应</span><span class="sxs-lookup"><span data-stu-id="8a323-125">Response</span></span>

<span data-ttu-id="8a323-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8a323-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a323-128">示例</span><span class="sxs-lookup"><span data-stu-id="8a323-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a323-129">请求</span><span class="sxs-lookup"><span data-stu-id="8a323-129">Request</span></span>

<span data-ttu-id="8a323-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a323-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8a323-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8a323-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a323-132">C#</span><span class="sxs-lookup"><span data-stu-id="8a323-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a323-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a323-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a323-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="8a323-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a323-135">响应</span><span class="sxs-lookup"><span data-stu-id="8a323-135">Response</span></span>

<span data-ttu-id="8a323-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a323-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
