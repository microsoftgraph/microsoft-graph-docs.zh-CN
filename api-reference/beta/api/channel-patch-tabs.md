---
title: 更新选项卡
description: 更新指定选项卡的属性。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 121c9805b099aeb1d84843d085948f20695e6c7b
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607502"
---
# <a name="update-tab"></a><span data-ttu-id="a5550-103">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="a5550-103">Update tab</span></span>

<span data-ttu-id="a5550-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5550-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5550-105">更新指定 [选项卡](../resources/teamstab.md)的属性。这可用于配置选项卡的内容。</span><span class="sxs-lookup"><span data-stu-id="a5550-105">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5550-106">权限</span><span class="sxs-lookup"><span data-stu-id="a5550-106">Permissions</span></span>
<span data-ttu-id="a5550-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5550-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5550-109">Permission type</span></span>      | <span data-ttu-id="a5550-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5550-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5550-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5550-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5550-112">TeamsTab、ReadWriteForTeam、TeamsTab、all、All、All、All</span><span class="sxs-lookup"><span data-stu-id="a5550-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a5550-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5550-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5550-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5550-114">Not supported.</span></span>    |
|<span data-ttu-id="a5550-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5550-115">Application</span></span> | <span data-ttu-id="a5550-116">TeamsTab \*、TeamsTab、ReadWriteForTeam、Group、all、all、all、all 和 All。 All</span><span class="sxs-lookup"><span data-stu-id="a5550-116">TeamsTab.ReadWrite.Group\*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a5550-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="a5550-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="a5550-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a5550-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a5550-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="a5550-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5550-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5550-120">HTTP request</span></span>
```http
PATCH /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="a5550-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5550-121">Request headers</span></span>
| <span data-ttu-id="a5550-122">标头</span><span class="sxs-lookup"><span data-stu-id="a5550-122">Header</span></span>       | <span data-ttu-id="a5550-123">值</span><span class="sxs-lookup"><span data-stu-id="a5550-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5550-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5550-124">Authorization</span></span>  | <span data-ttu-id="a5550-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5550-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5550-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5550-127">Content-Type</span></span>  | <span data-ttu-id="a5550-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a5550-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5550-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5550-129">Request body</span></span>
<span data-ttu-id="a5550-130">在请求正文中，提供 [tab](../resources/teamstab.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5550-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a5550-131">响应</span><span class="sxs-lookup"><span data-stu-id="a5550-131">Response</span></span>

<span data-ttu-id="a5550-132">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a5550-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5550-133">示例</span><span class="sxs-lookup"><span data-stu-id="a5550-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a5550-134">请求</span><span class="sxs-lookup"><span data-stu-id="a5550-134">Request</span></span>
<span data-ttu-id="a5550-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a5550-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="a5550-136">响应</span><span class="sxs-lookup"><span data-stu-id="a5550-136">Response</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="a5550-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a5550-137">See also</span></span>

[<span data-ttu-id="a5550-138">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="a5550-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


