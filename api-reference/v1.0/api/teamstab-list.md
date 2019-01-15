---
title: 在通道列表选项卡
description: '检索团队中指定的通道中的选项卡的列表。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d731ff9218efd5db240084a462b2acf08641c46b
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016630"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="c1962-103">在通道列表选项卡</span><span class="sxs-lookup"><span data-stu-id="c1962-103">List tabs in channel</span></span>



<span data-ttu-id="c1962-104">检索指定的[频道](../resources/channel.md)中[团队](../resources/team.md)中的[选项卡](../resources/teamstab.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="c1962-104">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c1962-105">权限</span><span class="sxs-lookup"><span data-stu-id="c1962-105">Permissions</span></span>
<span data-ttu-id="c1962-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1962-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1962-108">Permission type</span></span>      | <span data-ttu-id="c1962-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1962-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1962-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1962-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1962-111">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1962-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="c1962-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1962-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1962-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1962-113">Not supported.</span></span>    |
| <span data-ttu-id="c1962-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1962-114">Application</span></span>                            | <span data-ttu-id="c1962-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1962-115">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="c1962-116">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="c1962-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c1962-117">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="c1962-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c1962-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1962-118">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1962-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1962-119">Optional query parameters</span></span>

<span data-ttu-id="c1962-120">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="c1962-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1962-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1962-121">Request headers</span></span>
| <span data-ttu-id="c1962-122">标头</span><span class="sxs-lookup"><span data-stu-id="c1962-122">Header</span></span>       | <span data-ttu-id="c1962-123">值</span><span class="sxs-lookup"><span data-stu-id="c1962-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1962-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1962-124">Authorization</span></span>  | <span data-ttu-id="c1962-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1962-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1962-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1962-127">Request body</span></span>
<span data-ttu-id="c1962-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1962-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1962-129">响应</span><span class="sxs-lookup"><span data-stu-id="c1962-129">Response</span></span>
<span data-ttu-id="c1962-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[选项卡](../resources/teamstab.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c1962-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1962-131">示例</span><span class="sxs-lookup"><span data-stu-id="c1962-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c1962-132">请求</span><span class="sxs-lookup"><span data-stu-id="c1962-132">Request</span></span>
<span data-ttu-id="c1962-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1962-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="c1962-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1962-134">Response</span></span>
<span data-ttu-id="c1962-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1962-135">The following is an example of the response.</span></span>
><span data-ttu-id="c1962-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1962-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "name": "My Contoso Tab - updated",
      "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": 20,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
