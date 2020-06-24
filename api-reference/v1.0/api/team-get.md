---
title: 获取团队
description: 检索指定团队的属性和关系。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc9a45e22022b6f95ab0e7dde4187bfe105af093
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845797"
---
# <a name="get-team"></a><span data-ttu-id="c24d0-103">获取团队</span><span class="sxs-lookup"><span data-stu-id="c24d0-103">Get team</span></span>

<span data-ttu-id="c24d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c24d0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="c24d0-105">检索指定[团队](../resources/team.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c24d0-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c24d0-106">权限</span><span class="sxs-lookup"><span data-stu-id="c24d0-106">Permissions</span></span>
<span data-ttu-id="c24d0-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c24d0-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c24d0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c24d0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c24d0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c24d0-109">Permission type</span></span>      | <span data-ttu-id="c24d0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c24d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c24d0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c24d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c24d0-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24d0-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c24d0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c24d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c24d0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c24d0-114">Not supported.</span></span>    |
|<span data-ttu-id="c24d0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c24d0-115">Application</span></span> | <span data-ttu-id="c24d0-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24d0-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c24d0-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="c24d0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c24d0-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="c24d0-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c24d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c24d0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c24d0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c24d0-120">Optional query parameters</span></span>
<span data-ttu-id="c24d0-121">此方法支持 $select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c24d0-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c24d0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c24d0-122">Request headers</span></span>
| <span data-ttu-id="c24d0-123">标头</span><span class="sxs-lookup"><span data-stu-id="c24d0-123">Header</span></span>       | <span data-ttu-id="c24d0-124">值</span><span class="sxs-lookup"><span data-stu-id="c24d0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c24d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c24d0-125">Authorization</span></span>  | <span data-ttu-id="c24d0-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c24d0-126">Bearer {token}.</span></span> <span data-ttu-id="c24d0-127">Required.</span><span class="sxs-lookup"><span data-stu-id="c24d0-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c24d0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c24d0-128">Request body</span></span>
<span data-ttu-id="c24d0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c24d0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c24d0-130">响应</span><span class="sxs-lookup"><span data-stu-id="c24d0-130">Response</span></span>

<span data-ttu-id="c24d0-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [team](../resources/team.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c24d0-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c24d0-132">示例</span><span class="sxs-lookup"><span data-stu-id="c24d0-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c24d0-133">请求</span><span class="sxs-lookup"><span data-stu-id="c24d0-133">Request</span></span>
<span data-ttu-id="c24d0-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c24d0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c24d0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c24d0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}
```
# <a name="c"></a>[<span data-ttu-id="c24d0-136">C#</span><span class="sxs-lookup"><span data-stu-id="c24d0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c24d0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c24d0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c24d0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c24d0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c24d0-139">Java</span><span class="sxs-lookup"><span data-stu-id="c24d0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c24d0-140">响应</span><span class="sxs-lookup"><span data-stu-id="c24d0-140">Response</span></span>
<span data-ttu-id="c24d0-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c24d0-141">The following is an example of the response.</span></span> 

><span data-ttu-id="c24d0-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="c24d0-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c24d0-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c24d0-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived": false,
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  },
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
