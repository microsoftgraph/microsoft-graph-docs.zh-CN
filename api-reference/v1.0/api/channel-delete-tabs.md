---
title: 从频道中删除选项卡
description: '从 (频道) 取消固定选项卡。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e7b2b5404328f659512ff246ed7207be23735583
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971382"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="40810-103">从频道中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="40810-103">Delete tab from channel</span></span>

<span data-ttu-id="40810-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40810-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="40810-105">从 (团队) 频道中删除取消固定选项卡[。](../resources/team.md) [](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="40810-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="40810-106">权限</span><span class="sxs-lookup"><span data-stu-id="40810-106">Permissions</span></span>
<span data-ttu-id="40810-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40810-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40810-109">Permission type</span></span>      | <span data-ttu-id="40810-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40810-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40810-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40810-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="40810-112">TeamsTab.ReadWriteForTeam、TeamsTab.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40810-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="40810-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40810-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40810-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40810-114">Not supported.</span></span>    |
|<span data-ttu-id="40810-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40810-115">Application</span></span> | <span data-ttu-id="40810-116">TeamsTab.Delete.Group、TeamsTab.ReadWrite.Group、TeamsTab.ReadWriteForTeam.All、TeamsTab.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40810-116">TeamsTab.Delete.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="40810-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="40810-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="40810-p102">**注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="40810-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="40810-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40810-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="40810-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="40810-121">Request headers</span></span>
| <span data-ttu-id="40810-122">标头</span><span class="sxs-lookup"><span data-stu-id="40810-122">Header</span></span>       | <span data-ttu-id="40810-123">值</span><span class="sxs-lookup"><span data-stu-id="40810-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40810-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="40810-124">Authorization</span></span>  | <span data-ttu-id="40810-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40810-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40810-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40810-127">Request body</span></span>
<span data-ttu-id="40810-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40810-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40810-129">响应</span><span class="sxs-lookup"><span data-stu-id="40810-129">Response</span></span>

<span data-ttu-id="40810-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="40810-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40810-132">示例</span><span class="sxs-lookup"><span data-stu-id="40810-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="40810-133">请求</span><span class="sxs-lookup"><span data-stu-id="40810-133">Request</span></span>
<span data-ttu-id="40810-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40810-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="40810-135">响应</span><span class="sxs-lookup"><span data-stu-id="40810-135">Response</span></span>
<span data-ttu-id="40810-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40810-136">The following is an example of the response.</span></span> <span data-ttu-id="40810-137">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="40810-137">Note: The response object shown here might be shortened for readability.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

