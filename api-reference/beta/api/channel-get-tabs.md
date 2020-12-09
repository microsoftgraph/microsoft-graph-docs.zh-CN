---
title: 通道中的获取选项卡
description: '在团队内的频道中检索指定选项卡的属性和关系。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee05de9b1fcfea9bd08c98ccf3f8a491b34c0399
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607536"
---
# <a name="get-tab-in-channel"></a><span data-ttu-id="428dd-103">通道中的获取选项卡</span><span class="sxs-lookup"><span data-stu-id="428dd-103">Get tab in channel</span></span>

<span data-ttu-id="428dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="428dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="428dd-105">在[团队](../resources/team.md)内的[频道](../resources/channel.md)中检索指定[选项卡](../resources/teamstab.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="428dd-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="428dd-106">权限</span><span class="sxs-lookup"><span data-stu-id="428dd-106">Permissions</span></span>
<span data-ttu-id="428dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="428dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="428dd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="428dd-109">Permission type</span></span>      | <span data-ttu-id="428dd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="428dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="428dd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="428dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="428dd-112">TeamsTab、TeamsTab、ReadWriteForTeam、TeamsTab、Group. all、、、、all、all、all 和 All 的所有读写</span><span class="sxs-lookup"><span data-stu-id="428dd-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="428dd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="428dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="428dd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="428dd-114">Not supported.</span></span>    |
|<span data-ttu-id="428dd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="428dd-115">Application</span></span> | <span data-ttu-id="428dd-116">TeamsTab、*TeamsTab*、TeamsTab、TeamsTab、group、Group、Group、group。 all、、、、all、all、、all、all、all、All 和 all</span><span class="sxs-lookup"><span data-stu-id="428dd-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="428dd-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="428dd-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="428dd-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="428dd-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="428dd-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="428dd-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="428dd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="428dd-120">HTTP request</span></span>
```http
GET /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="428dd-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="428dd-121">Optional query parameters</span></span>

<span data-ttu-id="428dd-122">此方法支持 $select 和 $expand [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="428dd-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="428dd-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="428dd-123">Request headers</span></span>
| <span data-ttu-id="428dd-124">标头</span><span class="sxs-lookup"><span data-stu-id="428dd-124">Header</span></span>       | <span data-ttu-id="428dd-125">值</span><span class="sxs-lookup"><span data-stu-id="428dd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="428dd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="428dd-126">Authorization</span></span>  | <span data-ttu-id="428dd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="428dd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="428dd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="428dd-129">Request body</span></span>
<span data-ttu-id="428dd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="428dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="428dd-131">响应</span><span class="sxs-lookup"><span data-stu-id="428dd-131">Response</span></span>

<span data-ttu-id="428dd-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [tab](../resources/teamstab.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="428dd-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="428dd-133">示例</span><span class="sxs-lookup"><span data-stu-id="428dd-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="428dd-134">请求</span><span class="sxs-lookup"><span data-stu-id="428dd-134">Request</span></span>
<span data-ttu-id="428dd-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="428dd-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="428dd-136">响应</span><span class="sxs-lookup"><span data-stu-id="428dd-136">Response</span></span>
<span data-ttu-id="428dd-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="428dd-137">The following is an example of the response.</span></span> 

><span data-ttu-id="428dd-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="428dd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


