---
title: teamsAppInstallation in team： upgrade
description: 升级团队中的应用安装
author: akjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c3df922e9fc15238bb5531fc38a935f613b1c98
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060021"
---
# <a name="teamsappinstallation-in-team-upgrade"></a><span data-ttu-id="00f4c-103">teamsAppInstallation in team： upgrade</span><span class="sxs-lookup"><span data-stu-id="00f4c-103">teamsAppInstallation in team: upgrade</span></span>

<span data-ttu-id="00f4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00f4c-105">将 [团队中的](../resources/teamsappinstallation.md) 应用 [安装升级到](../resources/team.md) 应用的最新版本。</span><span class="sxs-lookup"><span data-stu-id="00f4c-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="00f4c-106">权限</span><span class="sxs-lookup"><span data-stu-id="00f4c-106">Permissions</span></span>

<span data-ttu-id="00f4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00f4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f4c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="00f4c-109">Permission type</span></span>      | <span data-ttu-id="00f4c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00f4c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00f4c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00f4c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00f4c-112">TeamsAppInstallation.ReadWriteForTeam、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f4c-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="00f4c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00f4c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00f4c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="00f4c-114">Not supported.</span></span>    |
|<span data-ttu-id="00f4c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="00f4c-115">Application</span></span> | <span data-ttu-id="00f4c-116">TeamsAppInstallation.ReadWriteForTeam.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f4c-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00f4c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00f4c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="00f4c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="00f4c-118">Request headers</span></span>

| <span data-ttu-id="00f4c-119">标头</span><span class="sxs-lookup"><span data-stu-id="00f4c-119">Header</span></span>       | <span data-ttu-id="00f4c-120">值</span><span class="sxs-lookup"><span data-stu-id="00f4c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00f4c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00f4c-121">Authorization</span></span>  | <span data-ttu-id="00f4c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00f4c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00f4c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="00f4c-124">Request body</span></span>

<span data-ttu-id="00f4c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="00f4c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00f4c-126">响应</span><span class="sxs-lookup"><span data-stu-id="00f4c-126">Response</span></span>

<span data-ttu-id="00f4c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="00f4c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00f4c-129">示例</span><span class="sxs-lookup"><span data-stu-id="00f4c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="00f4c-130">请求</span><span class="sxs-lookup"><span data-stu-id="00f4c-130">Request</span></span>

<span data-ttu-id="00f4c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00f4c-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="00f4c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="00f4c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp_in_team"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade
```
# <a name="c"></a>[<span data-ttu-id="00f4c-133">C#</span><span class="sxs-lookup"><span data-stu-id="00f4c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00f4c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00f4c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00f4c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00f4c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00f4c-136">Java</span><span class="sxs-lookup"><span data-stu-id="00f4c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="00f4c-137">响应</span><span class="sxs-lookup"><span data-stu-id="00f4c-137">Response</span></span>

<span data-ttu-id="00f4c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="00f4c-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp_in_team",
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
  "description": "Upgrade app in team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


