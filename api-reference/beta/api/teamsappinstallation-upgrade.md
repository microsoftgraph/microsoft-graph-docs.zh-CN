---
title: 升级团队中的应用程序
description: 升级团队中的应用程序安装
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 967eb8092e5cf7e971ecc690dded4dbae3578f52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999067"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="7fb31-103">升级团队中的应用程序</span><span class="sxs-lookup"><span data-stu-id="7fb31-103">Upgrade an app in a team</span></span>

<span data-ttu-id="7fb31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fb31-105">将[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7fb31-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fb31-106">权限</span><span class="sxs-lookup"><span data-stu-id="7fb31-106">Permissions</span></span>

<span data-ttu-id="7fb31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fb31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fb31-109">Permission type</span></span>      | <span data-ttu-id="7fb31-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fb31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fb31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fb31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7fb31-112">TeamsAppInstallation，ReadWriteForTeam，all，All，All</span><span class="sxs-lookup"><span data-stu-id="7fb31-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="7fb31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fb31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fb31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fb31-114">Not supported.</span></span>    |
|<span data-ttu-id="7fb31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fb31-115">Application</span></span> | <span data-ttu-id="7fb31-116">TeamsAppInstallation、ReadWriteForTeam、all、ReadWrite。所有</span><span class="sxs-lookup"><span data-stu-id="7fb31-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fb31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fb31-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="7fb31-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fb31-118">Request headers</span></span>

| <span data-ttu-id="7fb31-119">标头</span><span class="sxs-lookup"><span data-stu-id="7fb31-119">Header</span></span>       | <span data-ttu-id="7fb31-120">值</span><span class="sxs-lookup"><span data-stu-id="7fb31-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7fb31-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fb31-121">Authorization</span></span>  | <span data-ttu-id="7fb31-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fb31-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fb31-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fb31-124">Request body</span></span>

<span data-ttu-id="7fb31-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7fb31-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb31-126">响应</span><span class="sxs-lookup"><span data-stu-id="7fb31-126">Response</span></span>

<span data-ttu-id="7fb31-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7fb31-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb31-129">示例</span><span class="sxs-lookup"><span data-stu-id="7fb31-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fb31-130">请求</span><span class="sxs-lookup"><span data-stu-id="7fb31-130">Request</span></span>

<span data-ttu-id="7fb31-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7fb31-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fb31-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb31-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="7fb31-133">C#</span><span class="sxs-lookup"><span data-stu-id="7fb31-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fb31-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fb31-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fb31-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fb31-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fb31-136">响应</span><span class="sxs-lookup"><span data-stu-id="7fb31-136">Response</span></span>

<span data-ttu-id="7fb31-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7fb31-137">The following is an example of the response.</span></span> 

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


