---
title: 升级团队中的应用程序
description: 升级团队中的应用程序安装
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb2a97843dce69837eb4b294cd88ac5fd8b6db06
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313019"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="77cd4-103">升级团队中的应用程序</span><span class="sxs-lookup"><span data-stu-id="77cd4-103">Upgrade an app in a team</span></span>

<span data-ttu-id="77cd4-104">将[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="77cd4-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="77cd4-105">权限</span><span class="sxs-lookup"><span data-stu-id="77cd4-105">Permissions</span></span>

<span data-ttu-id="77cd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77cd4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77cd4-108">Permission type</span></span>      | <span data-ttu-id="77cd4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77cd4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77cd4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77cd4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77cd4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77cd4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="77cd4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77cd4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77cd4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77cd4-113">Not supported.</span></span>    |
|<span data-ttu-id="77cd4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77cd4-114">Application</span></span> | <span data-ttu-id="77cd4-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77cd4-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="77cd4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77cd4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="77cd4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="77cd4-117">Request headers</span></span>

| <span data-ttu-id="77cd4-118">标头</span><span class="sxs-lookup"><span data-stu-id="77cd4-118">Header</span></span>       | <span data-ttu-id="77cd4-119">值</span><span class="sxs-lookup"><span data-stu-id="77cd4-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77cd4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77cd4-120">Authorization</span></span>  | <span data-ttu-id="77cd4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77cd4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77cd4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="77cd4-123">Request body</span></span>

<span data-ttu-id="77cd4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77cd4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77cd4-125">响应</span><span class="sxs-lookup"><span data-stu-id="77cd4-125">Response</span></span>

<span data-ttu-id="77cd4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="77cd4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77cd4-128">示例</span><span class="sxs-lookup"><span data-stu-id="77cd4-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="77cd4-129">请求</span><span class="sxs-lookup"><span data-stu-id="77cd4-129">Request</span></span>

<span data-ttu-id="77cd4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77cd4-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="77cd4-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77cd4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77cd4-132">C#</span><span class="sxs-lookup"><span data-stu-id="77cd4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77cd4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77cd4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77cd4-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="77cd4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77cd4-135">Java</span><span class="sxs-lookup"><span data-stu-id="77cd4-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77cd4-136">响应</span><span class="sxs-lookup"><span data-stu-id="77cd4-136">Response</span></span>

<span data-ttu-id="77cd4-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77cd4-137">The following is an example of the response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
