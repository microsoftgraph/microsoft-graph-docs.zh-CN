---
title: 获取团队
description: 检索指定团队的属性和关系。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c8d1129c57444d95a1a3a46ee58590e102056a98
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290095"
---
# <a name="get-team"></a><span data-ttu-id="4dc44-103">获取团队</span><span class="sxs-lookup"><span data-stu-id="4dc44-103">Get team</span></span>

<span data-ttu-id="4dc44-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc44-105">检索指定[团队](../resources/team.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4dc44-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4dc44-106">权限</span><span class="sxs-lookup"><span data-stu-id="4dc44-106">Permissions</span></span>
<span data-ttu-id="4dc44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dc44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dc44-109">Permission type</span></span>      | <span data-ttu-id="4dc44-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dc44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dc44-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4dc44-112">User.readbasic.all、TeamSettings、TeamSettings、Group、group、group。 all、、、all、all、all、all 和 all。 all</span><span class="sxs-lookup"><span data-stu-id="4dc44-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4dc44-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dc44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dc44-114">Not supported.</span></span>    |
|<span data-ttu-id="4dc44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dc44-115">Application</span></span> | <span data-ttu-id="4dc44-116">TeamSettings、User.readbasic.all （[rsc](https://aka.ms/teams-rsc)）、TeamSettings、TeamSettings、、Group （RSC）、（[RSC](https://aka.ms/teams-rsc)）、、（全部）、、。 all，all，all： all，all。</span><span class="sxs-lookup"><span data-stu-id="4dc44-116">TeamSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="4dc44-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="4dc44-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4dc44-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="4dc44-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4dc44-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dc44-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4dc44-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4dc44-120">Optional query parameters</span></span>
<span data-ttu-id="4dc44-121">此方法支持 $select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4dc44-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dc44-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dc44-122">Request headers</span></span>
| <span data-ttu-id="4dc44-123">标头</span><span class="sxs-lookup"><span data-stu-id="4dc44-123">Header</span></span>       | <span data-ttu-id="4dc44-124">值</span><span class="sxs-lookup"><span data-stu-id="4dc44-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4dc44-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dc44-125">Authorization</span></span>  | <span data-ttu-id="4dc44-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4dc44-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4dc44-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dc44-128">Request body</span></span>
<span data-ttu-id="4dc44-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4dc44-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dc44-130">响应</span><span class="sxs-lookup"><span data-stu-id="4dc44-130">Response</span></span>

<span data-ttu-id="4dc44-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [team](../resources/team.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dc44-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4dc44-132">示例</span><span class="sxs-lookup"><span data-stu-id="4dc44-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4dc44-133">请求</span><span class="sxs-lookup"><span data-stu-id="4dc44-133">Request</span></span>
<span data-ttu-id="4dc44-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4dc44-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="4dc44-135">响应</span><span class="sxs-lookup"><span data-stu-id="4dc44-135">Response</span></span>
<span data-ttu-id="4dc44-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4dc44-136">The following is an example of the response.</span></span> 

><span data-ttu-id="4dc44-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4dc44-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
