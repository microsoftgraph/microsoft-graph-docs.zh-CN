---
title: 更新团队
description: 更新指定的团队的属性。
ms.openlocfilehash: 23f65ef1cd1948941bd814a521bdaa0984553dff
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222602"
---
# <a name="update-team"></a><span data-ttu-id="2b985-103">更新团队</span><span class="sxs-lookup"><span data-stu-id="2b985-103">Update team</span></span>



<span data-ttu-id="2b985-104">更新指定的[团队](../resources/team.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="2b985-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b985-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b985-105">Permissions</span></span>
<span data-ttu-id="2b985-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b985-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b985-108">Permission type</span></span>      | <span data-ttu-id="2b985-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b985-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b985-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b985-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b985-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b985-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b985-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b985-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b985-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b985-113">Not supported.</span></span>    |
|<span data-ttu-id="2b985-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b985-114">Application</span></span> | <span data-ttu-id="2b985-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b985-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="2b985-116">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="2b985-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2b985-117">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="2b985-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b985-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b985-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b985-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b985-119">Request headers</span></span>
| <span data-ttu-id="2b985-120">标头</span><span class="sxs-lookup"><span data-stu-id="2b985-120">Header</span></span>       | <span data-ttu-id="2b985-121">值</span><span class="sxs-lookup"><span data-stu-id="2b985-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b985-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b985-122">Authorization</span></span>  | <span data-ttu-id="2b985-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b985-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b985-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b985-125">Content-Type</span></span>  | <span data-ttu-id="2b985-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b985-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b985-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b985-127">Request body</span></span>
<span data-ttu-id="2b985-128">在请求正文中，提供[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b985-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2b985-129">响应</span><span class="sxs-lookup"><span data-stu-id="2b985-129">Response</span></span>

<span data-ttu-id="2b985-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2b985-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2b985-131">示例</span><span class="sxs-lookup"><span data-stu-id="2b985-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2b985-132">请求</span><span class="sxs-lookup"><span data-stu-id="2b985-132">Request</span></span>
<span data-ttu-id="2b985-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2b985-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="2b985-134">响应</span><span class="sxs-lookup"><span data-stu-id="2b985-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
