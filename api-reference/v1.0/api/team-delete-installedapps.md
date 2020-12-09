---
title: 从团队中删除应用
description: 从指定的团队中卸载应用程序。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 159f355514cab6f1ffb230f26c95208e58e416b6
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607340"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="8341c-103">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="8341c-103">Remove app from team</span></span>

<span data-ttu-id="8341c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8341c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8341c-105">从指定的[团队](../resources/team.md)中卸载[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="8341c-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8341c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8341c-106">Permissions</span></span>

<span data-ttu-id="8341c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8341c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8341c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8341c-109">Permission type</span></span>      | <span data-ttu-id="8341c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8341c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8341c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8341c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8341c-112">TeamsAppInstallation，ReadWriteForTeam，all，All，All</span><span class="sxs-lookup"><span data-stu-id="8341c-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8341c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8341c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8341c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8341c-114">Not supported.</span></span>    |
|<span data-ttu-id="8341c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8341c-115">Application</span></span> | <span data-ttu-id="8341c-116">TeamsAppInstallation、ReadWriteForTeam、all、ReadWrite。所有</span><span class="sxs-lookup"><span data-stu-id="8341c-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8341c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8341c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="8341c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8341c-118">Request headers</span></span>

| <span data-ttu-id="8341c-119">标头</span><span class="sxs-lookup"><span data-stu-id="8341c-119">Header</span></span>       | <span data-ttu-id="8341c-120">值</span><span class="sxs-lookup"><span data-stu-id="8341c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8341c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8341c-121">Authorization</span></span>  | <span data-ttu-id="8341c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8341c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8341c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8341c-124">Request body</span></span>

<span data-ttu-id="8341c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8341c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8341c-126">响应</span><span class="sxs-lookup"><span data-stu-id="8341c-126">Response</span></span>

<span data-ttu-id="8341c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8341c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8341c-129">示例</span><span class="sxs-lookup"><span data-stu-id="8341c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8341c-130">请求</span><span class="sxs-lookup"><span data-stu-id="8341c-130">Request</span></span>

<span data-ttu-id="8341c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8341c-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp_in_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```

### <a name="response"></a><span data-ttu-id="8341c-132">响应</span><span class="sxs-lookup"><span data-stu-id="8341c-132">Response</span></span>

<span data-ttu-id="8341c-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8341c-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp_in_team",
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
  "description": "Remove app from team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


