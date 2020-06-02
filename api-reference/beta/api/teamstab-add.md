---
title: 将选项卡添加到频道
description: '将选项卡添加（固定）到团队中的指定频道。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c06edf2a9a98fcda693f9738cbf1133f089f785
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491733"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="0a841-103">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="0a841-103">Add tab to channel</span></span>

<span data-ttu-id="0a841-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a841-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a841-105">将[选项卡](../resources/teamstab.md)添加（固定）到[团队](../resources/team.md)中的指定[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="0a841-105">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="0a841-106">相应的应用必须事先[安装在团队中](../api/teamsappinstallation-add.md)。</span><span class="sxs-lookup"><span data-stu-id="0a841-106">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a841-107">权限</span><span class="sxs-lookup"><span data-stu-id="0a841-107">Permissions</span></span>
<span data-ttu-id="0a841-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a841-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a841-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a841-110">Permission type</span></span>      | <span data-ttu-id="0a841-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a841-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a841-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a841-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0a841-113">TeamsTab，TeamsTab，all，all，All，All，All</span><span class="sxs-lookup"><span data-stu-id="0a841-113">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0a841-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a841-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a841-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a841-115">Not supported.</span></span>    |
| <span data-ttu-id="0a841-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a841-116">Application</span></span>                            | <span data-ttu-id="0a841-117">TeamsTab \*、TeamsTab、TeamsTab、Group、all、all、all、All、All</span><span class="sxs-lookup"><span data-stu-id="0a841-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0a841-118">**注意**：标记为 \* 的权限使用[特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="0a841-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="0a841-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0a841-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0a841-120">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="0a841-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0a841-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a841-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="0a841-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a841-122">Request headers</span></span>
| <span data-ttu-id="0a841-123">标头</span><span class="sxs-lookup"><span data-stu-id="0a841-123">Header</span></span>       | <span data-ttu-id="0a841-124">值</span><span class="sxs-lookup"><span data-stu-id="0a841-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a841-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a841-125">Authorization</span></span>  | <span data-ttu-id="0a841-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a841-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a841-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a841-128">Request body</span></span>

<span data-ttu-id="0a841-129">一个 [teamsTab](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="0a841-129">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="0a841-130">响应</span><span class="sxs-lookup"><span data-stu-id="0a841-130">Response</span></span>

<span data-ttu-id="0a841-131">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0a841-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a841-132">示例</span><span class="sxs-lookup"><span data-stu-id="0a841-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0a841-133">请求</span><span class="sxs-lookup"><span data-stu-id="0a841-133">Request</span></span>

<span data-ttu-id="0a841-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a841-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="0a841-135">响应</span><span class="sxs-lookup"><span data-stu-id="0a841-135">Response</span></span>

<span data-ttu-id="0a841-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0a841-136">The following is an example of the response.</span></span> <span data-ttu-id="0a841-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a841-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a841-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0a841-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="0a841-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0a841-139">See also</span></span>

[<span data-ttu-id="0a841-140">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="0a841-140">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
