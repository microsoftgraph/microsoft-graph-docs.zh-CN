---
title: 更新团队
description: 更新指定的团队的属性。
author: nkramer
ms.openlocfilehash: 19a3c55295bc54fcd7f1c9e24f88e386fc4dc2bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331918"
---
# <a name="update-team"></a><span data-ttu-id="89114-103">更新团队</span><span class="sxs-lookup"><span data-stu-id="89114-103">Update team</span></span>

> <span data-ttu-id="89114-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89114-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89114-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89114-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89114-106">更新指定的[团队](../resources/team.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="89114-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89114-107">权限</span><span class="sxs-lookup"><span data-stu-id="89114-107">Permissions</span></span>
<span data-ttu-id="89114-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89114-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89114-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="89114-110">Permission type</span></span>      | <span data-ttu-id="89114-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89114-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89114-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89114-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89114-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89114-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="89114-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89114-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89114-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="89114-115">Not supported.</span></span>    |
|<span data-ttu-id="89114-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="89114-116">Application</span></span> | <span data-ttu-id="89114-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89114-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="89114-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="89114-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="89114-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="89114-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="89114-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89114-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="89114-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="89114-121">Request headers</span></span>
| <span data-ttu-id="89114-122">标头</span><span class="sxs-lookup"><span data-stu-id="89114-122">Header</span></span>       | <span data-ttu-id="89114-123">值</span><span class="sxs-lookup"><span data-stu-id="89114-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89114-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89114-124">Authorization</span></span>  | <span data-ttu-id="89114-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89114-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89114-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89114-127">Content-Type</span></span>  | <span data-ttu-id="89114-128">application/json</span><span class="sxs-lookup"><span data-stu-id="89114-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89114-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="89114-129">Request body</span></span>
<span data-ttu-id="89114-130">在请求正文中，提供[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89114-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="89114-131">响应</span><span class="sxs-lookup"><span data-stu-id="89114-131">Response</span></span>

<span data-ttu-id="89114-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="89114-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="89114-133">示例</span><span class="sxs-lookup"><span data-stu-id="89114-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="89114-134">请求</span><span class="sxs-lookup"><span data-stu-id="89114-134">Request</span></span>
<span data-ttu-id="89114-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89114-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="89114-136">响应</span><span class="sxs-lookup"><span data-stu-id="89114-136">Response</span></span>
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
