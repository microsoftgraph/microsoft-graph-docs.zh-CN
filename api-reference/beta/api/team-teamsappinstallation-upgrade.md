---
title: teamsAppInstallation： upgrade
description: 升级团队中的应用程序安装
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05b275469e44c2915b60df4c08ac04048147ef3d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607568"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="9af33-103">teamsAppInstallation： upgrade</span><span class="sxs-lookup"><span data-stu-id="9af33-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="9af33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9af33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9af33-105">将[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9af33-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="9af33-106">权限</span><span class="sxs-lookup"><span data-stu-id="9af33-106">Permissions</span></span>

<span data-ttu-id="9af33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9af33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9af33-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9af33-109">Permission type</span></span>      | <span data-ttu-id="9af33-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9af33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9af33-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9af33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9af33-112">TeamsAppInstallation，ReadWriteForTeam，all，All，All</span><span class="sxs-lookup"><span data-stu-id="9af33-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9af33-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9af33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9af33-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9af33-114">Not supported.</span></span>    |
|<span data-ttu-id="9af33-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9af33-115">Application</span></span> | <span data-ttu-id="9af33-116">TeamsAppInstallation、ReadWriteForTeam、all、ReadWrite。所有</span><span class="sxs-lookup"><span data-stu-id="9af33-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9af33-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9af33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="9af33-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9af33-118">Request headers</span></span>

| <span data-ttu-id="9af33-119">标头</span><span class="sxs-lookup"><span data-stu-id="9af33-119">Header</span></span>       | <span data-ttu-id="9af33-120">值</span><span class="sxs-lookup"><span data-stu-id="9af33-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9af33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9af33-121">Authorization</span></span>  | <span data-ttu-id="9af33-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9af33-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9af33-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9af33-124">Request body</span></span>

<span data-ttu-id="9af33-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9af33-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9af33-126">响应</span><span class="sxs-lookup"><span data-stu-id="9af33-126">Response</span></span>

<span data-ttu-id="9af33-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9af33-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9af33-129">示例</span><span class="sxs-lookup"><span data-stu-id="9af33-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9af33-130">请求</span><span class="sxs-lookup"><span data-stu-id="9af33-130">Request</span></span>

<span data-ttu-id="9af33-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9af33-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp_in_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade
```


### <a name="response"></a><span data-ttu-id="9af33-132">响应</span><span class="sxs-lookup"><span data-stu-id="9af33-132">Response</span></span>

<span data-ttu-id="9af33-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9af33-133">The following is an example of the response.</span></span> 

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


