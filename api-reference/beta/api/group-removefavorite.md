---
title: 'group: removeFavorite'
description: 从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: c6e1d81f9b6b95a3122850d09b918e33e07b6dd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324157"
---
# <a name="group-removefavorite"></a><span data-ttu-id="f9ac1-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="f9ac1-104">group: removeFavorite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ac1-p102">从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-p102">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9ac1-107">权限</span><span class="sxs-lookup"><span data-stu-id="f9ac1-107">Permissions</span></span>
<span data-ttu-id="f9ac1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ac1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9ac1-110">Permission type</span></span>      | <span data-ttu-id="f9ac1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9ac1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ac1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9ac1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9ac1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ac1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9ac1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9ac1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ac1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-115">Not supported.</span></span>    |
|<span data-ttu-id="f9ac1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9ac1-116">Application</span></span> | <span data-ttu-id="f9ac1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ac1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9ac1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="f9ac1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9ac1-119">Request headers</span></span>
| <span data-ttu-id="f9ac1-120">标头</span><span class="sxs-lookup"><span data-stu-id="f9ac1-120">Header</span></span>       | <span data-ttu-id="f9ac1-121">值</span><span class="sxs-lookup"><span data-stu-id="f9ac1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9ac1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9ac1-122">Authorization</span></span>  | <span data-ttu-id="f9ac1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9ac1-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="f9ac1-125">Prefer</span></span> | <span data-ttu-id="f9ac1-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-126">return=minimal.</span></span> <span data-ttu-id="f9ac1-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f9ac1-128">可选。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f9ac1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9ac1-129">Request body</span></span>
<span data-ttu-id="f9ac1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ac1-131">响应</span><span class="sxs-lookup"><span data-stu-id="f9ac1-131">Response</span></span>
<span data-ttu-id="f9ac1-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9ac1-134">示例</span><span class="sxs-lookup"><span data-stu-id="f9ac1-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9ac1-135">请求</span><span class="sxs-lookup"><span data-stu-id="f9ac1-135">Request</span></span>
<span data-ttu-id="f9ac1-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="f9ac1-137">响应</span><span class="sxs-lookup"><span data-stu-id="f9ac1-137">Response</span></span>
<span data-ttu-id="f9ac1-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f9ac1-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
