---
title: 获取工作组
description: 检索的属性和指定团队的关系。
author: nkramer
ms.openlocfilehash: dfa59948a9bffce77c98a3462f919e75fe18042e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329230"
---
# <a name="get-team"></a><span data-ttu-id="868d6-103">获取工作组</span><span class="sxs-lookup"><span data-stu-id="868d6-103">Get team</span></span>

> <span data-ttu-id="868d6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="868d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="868d6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="868d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="868d6-106">检索的属性和指定[团队](../resources/team.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="868d6-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="868d6-107">权限</span><span class="sxs-lookup"><span data-stu-id="868d6-107">Permissions</span></span>
<span data-ttu-id="868d6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="868d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="868d6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="868d6-110">Permission type</span></span>      | <span data-ttu-id="868d6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="868d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="868d6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="868d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="868d6-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="868d6-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="868d6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="868d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="868d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="868d6-115">Not supported.</span></span>    |
|<span data-ttu-id="868d6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="868d6-116">Application</span></span> | <span data-ttu-id="868d6-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="868d6-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="868d6-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="868d6-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="868d6-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="868d6-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="868d6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="868d6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="868d6-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="868d6-121">Optional query parameters</span></span>
<span data-ttu-id="868d6-122">此方法支持 $select 和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="868d6-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="868d6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="868d6-123">Request headers</span></span>
| <span data-ttu-id="868d6-124">标头</span><span class="sxs-lookup"><span data-stu-id="868d6-124">Header</span></span>       | <span data-ttu-id="868d6-125">值</span><span class="sxs-lookup"><span data-stu-id="868d6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="868d6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="868d6-126">Authorization</span></span>  | <span data-ttu-id="868d6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="868d6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="868d6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="868d6-129">Request body</span></span>
<span data-ttu-id="868d6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="868d6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="868d6-131">响应</span><span class="sxs-lookup"><span data-stu-id="868d6-131">Response</span></span>

<span data-ttu-id="868d6-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[团队](../resources/team.md)对象。</span><span class="sxs-lookup"><span data-stu-id="868d6-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="868d6-133">示例</span><span class="sxs-lookup"><span data-stu-id="868d6-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="868d6-134">请求</span><span class="sxs-lookup"><span data-stu-id="868d6-134">Request</span></span>
<span data-ttu-id="868d6-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="868d6-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="868d6-136">响应</span><span class="sxs-lookup"><span data-stu-id="868d6-136">Response</span></span>
<span data-ttu-id="868d6-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="868d6-137">The following is an example of the response.</span></span> 

><span data-ttu-id="868d6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="868d6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
