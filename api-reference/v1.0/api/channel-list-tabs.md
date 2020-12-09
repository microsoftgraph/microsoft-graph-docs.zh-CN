---
title: 通道中的列表选项卡
description: '检索团队中指定通道中的选项卡列表。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79dfc817aac163109352caf999b40870d672ca01
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607303"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="ac2f0-103">通道中的列表选项卡</span><span class="sxs-lookup"><span data-stu-id="ac2f0-103">List tabs in channel</span></span>

<span data-ttu-id="ac2f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac2f0-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="ac2f0-105">检索[团队](../resources/team.md)中指定[通道](../resources/channel.md)中的[选项卡](../resources/teamstab.md)列表。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-105">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ac2f0-106">权限</span><span class="sxs-lookup"><span data-stu-id="ac2f0-106">Permissions</span></span>
<span data-ttu-id="ac2f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac2f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac2f0-109">Permission type</span></span>      | <span data-ttu-id="ac2f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac2f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac2f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac2f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ac2f0-112">TeamsTab、TeamsTab、ReadWriteForTeam、TeamsTab、Group. all、、、、all、all、all 和 All 的所有读写</span><span class="sxs-lookup"><span data-stu-id="ac2f0-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ac2f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac2f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac2f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-114">Not supported.</span></span>    |
|<span data-ttu-id="ac2f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac2f0-115">Application</span></span> | <span data-ttu-id="ac2f0-116">TeamsTab、*TeamsTab*、TeamsTab、TeamsTab、group、Group、Group、group。 all、、、、all、all、、all、all、all、All 和 all</span><span class="sxs-lookup"><span data-stu-id="ac2f0-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ac2f0-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="ac2f0-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ac2f0-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ac2f0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac2f0-120">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac2f0-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ac2f0-121">Optional query parameters</span></span>

<span data-ttu-id="ac2f0-122">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac2f0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac2f0-123">Request headers</span></span>
| <span data-ttu-id="ac2f0-124">标头</span><span class="sxs-lookup"><span data-stu-id="ac2f0-124">Header</span></span>       | <span data-ttu-id="ac2f0-125">值</span><span class="sxs-lookup"><span data-stu-id="ac2f0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac2f0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac2f0-126">Authorization</span></span>  | <span data-ttu-id="ac2f0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac2f0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac2f0-129">Request body</span></span>
<span data-ttu-id="ac2f0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac2f0-131">响应</span><span class="sxs-lookup"><span data-stu-id="ac2f0-131">Response</span></span>
<span data-ttu-id="ac2f0-132">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和 [选项卡](../resources/teamstab.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-132">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac2f0-133">示例</span><span class="sxs-lookup"><span data-stu-id="ac2f0-133">Examples</span></span>

### <a name="example-1-list-all-the-tabs-in-the-channel-along-with-associated-teams-app"></a><span data-ttu-id="ac2f0-134">示例1：列出通道中的所有选项卡以及关联的团队应用</span><span class="sxs-lookup"><span data-stu-id="ac2f0-134">Example 1: List all the tabs in the channel along with associated Teams app</span></span>
#### <a name="request"></a><span data-ttu-id="ac2f0-135">请求</span><span class="sxs-lookup"><span data-stu-id="ac2f0-135">Request</span></span>
<span data-ttu-id="ac2f0-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tabs_in_channel_app_filter"
}
-->

```http
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs?$expand=teamsApp
```

#### <a name="response"></a><span data-ttu-id="ac2f0-137">响应</span><span class="sxs-lookup"><span data-stu-id="ac2f0-137">Response</span></span>
<span data-ttu-id="ac2f0-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-138">The following is an example of the response.</span></span>
><span data-ttu-id="ac2f0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": "20",
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```

### <a name="example-2-list-all-the-tabs-belonging-to-a-specific-app-in-a-channel"></a><span data-ttu-id="ac2f0-141">示例2：列出通道中的特定应用的所有选项卡</span><span class="sxs-lookup"><span data-stu-id="ac2f0-141">Example 2: List all the tabs belonging to a specific app in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="ac2f0-142">请求</span><span class="sxs-lookup"><span data-stu-id="ac2f0-142">Request</span></span>
<span data-ttu-id="ac2f0-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tabs_in_channel_app_filter"
}
-->

```http
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs?$expand=teamsApp&$filter=teamsApp/id eq 'com.microsoft.teamspace.tab.planner'
```

#### <a name="response"></a><span data-ttu-id="ac2f0-144">响应</span><span class="sxs-lookup"><span data-stu-id="ac2f0-144">Response</span></span>
<span data-ttu-id="ac2f0-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-145">The following is an example of the response.</span></span>
><span data-ttu-id="ac2f0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ac2f0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/channels('19%3A33b76eea88574bd1969dca37e2b7a819%40thread.skype')/tabs(teamsApp())",
  "@odata.count": 1,
  "value": [
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

