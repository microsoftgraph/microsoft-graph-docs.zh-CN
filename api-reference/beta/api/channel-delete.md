---
title: 删除通道
description: 删除通道。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2afd55c46228ecac38139657cdf51b1ce180cb13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936541"
---
# <a name="delete-channel"></a><span data-ttu-id="135af-103">删除通道</span><span class="sxs-lookup"><span data-stu-id="135af-103">Delete channel</span></span>

> <span data-ttu-id="135af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="135af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="135af-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="135af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="135af-106">删除[通道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="135af-106">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="135af-107">**注意**： 没有应用程序权限和此 API 的已知的问题。</span><span class="sxs-lookup"><span data-stu-id="135af-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="135af-108">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="135af-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="135af-109">权限</span><span class="sxs-lookup"><span data-stu-id="135af-109">Permissions</span></span>
<span data-ttu-id="135af-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="135af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="135af-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="135af-112">Permission type</span></span>      | <span data-ttu-id="135af-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="135af-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="135af-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="135af-114">Delegated (work or school account)</span></span> | <span data-ttu-id="135af-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="135af-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="135af-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="135af-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="135af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="135af-117">Not supported.</span></span>    |
|<span data-ttu-id="135af-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="135af-118">Application</span></span> | <span data-ttu-id="135af-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="135af-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="135af-120">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="135af-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="135af-121">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="135af-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="135af-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="135af-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="135af-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="135af-123">Request headers</span></span>
| <span data-ttu-id="135af-124">标头</span><span class="sxs-lookup"><span data-stu-id="135af-124">Header</span></span>       | <span data-ttu-id="135af-125">值</span><span class="sxs-lookup"><span data-stu-id="135af-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="135af-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="135af-126">Authorization</span></span>  | <span data-ttu-id="135af-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="135af-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="135af-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="135af-129">Request body</span></span>
<span data-ttu-id="135af-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="135af-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="135af-131">响应</span><span class="sxs-lookup"><span data-stu-id="135af-131">Response</span></span>

<span data-ttu-id="135af-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="135af-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="135af-134">示例</span><span class="sxs-lookup"><span data-stu-id="135af-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="135af-135">请求</span><span class="sxs-lookup"><span data-stu-id="135af-135">Request</span></span>
<span data-ttu-id="135af-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="135af-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="135af-137">响应</span><span class="sxs-lookup"><span data-stu-id="135af-137">Response</span></span>

<span data-ttu-id="135af-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="135af-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
