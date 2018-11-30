---
title: 选项卡添加到频道
description: '将 (pin) 添加到指定的通道团队中的一个选项卡。 '
ms.openlocfilehash: be246b0308be83e0b411fa89fe16034018756829
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043055"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="123d3-103">选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="123d3-103">Add tab to channel</span></span>

> <span data-ttu-id="123d3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="123d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="123d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="123d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="123d3-106">将 (pin) 添加到[团队](../resources/team.md)中指定的[频道](../resources/channel.md)一个[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="123d3-106">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="123d3-107">相应的应用程序已必须[安装在工作组中](../api/teamsappinstallation-add.md)。</span><span class="sxs-lookup"><span data-stu-id="123d3-107">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="123d3-108">权限</span><span class="sxs-lookup"><span data-stu-id="123d3-108">Permissions</span></span>
<span data-ttu-id="123d3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="123d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="123d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="123d3-111">Permission type</span></span>      | <span data-ttu-id="123d3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="123d3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="123d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="123d3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="123d3-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="123d3-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="123d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="123d3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="123d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="123d3-116">Not supported.</span></span>    |
| <span data-ttu-id="123d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="123d3-117">Application</span></span>                            | <span data-ttu-id="123d3-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="123d3-118">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="123d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="123d3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="123d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="123d3-120">Request headers</span></span>
| <span data-ttu-id="123d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="123d3-121">Header</span></span>       | <span data-ttu-id="123d3-122">值</span><span class="sxs-lookup"><span data-stu-id="123d3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="123d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="123d3-123">Authorization</span></span>  | <span data-ttu-id="123d3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="123d3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="123d3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="123d3-126">Request body</span></span>

<span data-ttu-id="123d3-127">[TeamsTab](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="123d3-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="123d3-128">响应</span><span class="sxs-lookup"><span data-stu-id="123d3-128">Response</span></span>

<span data-ttu-id="123d3-129">如果成功，此方法返回 `201 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="123d3-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="123d3-130">示例</span><span class="sxs-lookup"><span data-stu-id="123d3-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="123d3-131">请求</span><span class="sxs-lookup"><span data-stu-id="123d3-131">Request</span></span>

<span data-ttu-id="123d3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="123d3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="123d3-133">响应</span><span class="sxs-lookup"><span data-stu-id="123d3-133">Response</span></span>

<span data-ttu-id="123d3-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="123d3-134">The following is an example of the response.</span></span> <span data-ttu-id="123d3-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="123d3-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="123d3-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="123d3-136">All of the properties will be returned from an actual call.</span></span>
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
  "name": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="123d3-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="123d3-137">See also</span></span>

[<span data-ttu-id="123d3-138">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="123d3-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
