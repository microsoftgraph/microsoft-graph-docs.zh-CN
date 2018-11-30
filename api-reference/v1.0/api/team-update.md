---
title: 更新团队
description: 更新指定的团队的属性。
ms.openlocfilehash: 27cbf8f571752a27fb68727fe2695a0250f5dc75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007951"
---
# <a name="update-team"></a><span data-ttu-id="1f4c2-103">更新团队</span><span class="sxs-lookup"><span data-stu-id="1f4c2-103">Update team</span></span>



<span data-ttu-id="1f4c2-104">更新指定的[团队](../resources/team.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f4c2-105">权限</span><span class="sxs-lookup"><span data-stu-id="1f4c2-105">Permissions</span></span>
<span data-ttu-id="1f4c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1f4c2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f4c2-108">Permission type</span></span>      | <span data-ttu-id="1f4c2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f4c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f4c2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f4c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f4c2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f4c2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f4c2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f4c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f4c2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-113">Not supported.</span></span>    |
|<span data-ttu-id="1f4c2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f4c2-114">Application</span></span> | <span data-ttu-id="1f4c2-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f4c2-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="1f4c2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f4c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1f4c2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f4c2-117">Request headers</span></span>
| <span data-ttu-id="1f4c2-118">标头</span><span class="sxs-lookup"><span data-stu-id="1f4c2-118">Header</span></span>       | <span data-ttu-id="1f4c2-119">值</span><span class="sxs-lookup"><span data-stu-id="1f4c2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f4c2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f4c2-120">Authorization</span></span>  | <span data-ttu-id="1f4c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f4c2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f4c2-123">Content-Type</span></span>  | <span data-ttu-id="1f4c2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f4c2-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f4c2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f4c2-125">Request body</span></span>
<span data-ttu-id="1f4c2-126">在请求正文中，提供[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-126">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1f4c2-127">响应</span><span class="sxs-lookup"><span data-stu-id="1f4c2-127">Response</span></span>

<span data-ttu-id="1f4c2-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f4c2-129">示例</span><span class="sxs-lookup"><span data-stu-id="1f4c2-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1f4c2-130">请求</span><span class="sxs-lookup"><span data-stu-id="1f4c2-130">Request</span></span>
<span data-ttu-id="1f4c2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1f4c2-131">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="1f4c2-132">响应</span><span class="sxs-lookup"><span data-stu-id="1f4c2-132">Response</span></span>
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
