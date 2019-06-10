---
title: 获取团队
description: 检索指定团队的属性和关系。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 4a82949f717fd815aadb6423a7885b3ebe1da769
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812731"
---
# <a name="get-team"></a><span data-ttu-id="987c6-103">获取团队</span><span class="sxs-lookup"><span data-stu-id="987c6-103">Get team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="987c6-104">检索指定[团队](../resources/team.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="987c6-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="987c6-105">权限</span><span class="sxs-lookup"><span data-stu-id="987c6-105">Permissions</span></span>
<span data-ttu-id="987c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="987c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="987c6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="987c6-108">Permission type</span></span>      | <span data-ttu-id="987c6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="987c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="987c6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="987c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="987c6-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987c6-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="987c6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="987c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="987c6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="987c6-113">Not supported.</span></span>    |
|<span data-ttu-id="987c6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="987c6-114">Application</span></span> | <span data-ttu-id="987c6-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987c6-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="987c6-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="987c6-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="987c6-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="987c6-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="987c6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="987c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="987c6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="987c6-119">Optional query parameters</span></span>
<span data-ttu-id="987c6-120">此方法支持 $select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="987c6-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="987c6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="987c6-121">Request headers</span></span>
| <span data-ttu-id="987c6-122">标头</span><span class="sxs-lookup"><span data-stu-id="987c6-122">Header</span></span>       | <span data-ttu-id="987c6-123">值</span><span class="sxs-lookup"><span data-stu-id="987c6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="987c6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="987c6-124">Authorization</span></span>  | <span data-ttu-id="987c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="987c6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="987c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="987c6-127">Request body</span></span>
<span data-ttu-id="987c6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="987c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="987c6-129">响应</span><span class="sxs-lookup"><span data-stu-id="987c6-129">Response</span></span>

<span data-ttu-id="987c6-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [team](../resources/team.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="987c6-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="987c6-131">示例</span><span class="sxs-lookup"><span data-stu-id="987c6-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="987c6-132">请求</span><span class="sxs-lookup"><span data-stu-id="987c6-132">Request</span></span>
<span data-ttu-id="987c6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="987c6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="987c6-134">响应</span><span class="sxs-lookup"><span data-stu-id="987c6-134">Response</span></span>
<span data-ttu-id="987c6-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="987c6-135">The following is an example of the response.</span></span> 

><span data-ttu-id="987c6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="987c6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
