---
title: 删除通道
description: 删除通道。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 734df0a79881993f4e002562e5125305b624c4c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525330"
---
# <a name="delete-channel"></a><span data-ttu-id="e8a25-103">删除通道</span><span class="sxs-lookup"><span data-stu-id="e8a25-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8a25-104">删除[通道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="e8a25-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="e8a25-105">**注意**： 没有应用程序权限和此 API 的已知的问题。</span><span class="sxs-lookup"><span data-stu-id="e8a25-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="e8a25-106">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e8a25-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a25-107">权限</span><span class="sxs-lookup"><span data-stu-id="e8a25-107">Permissions</span></span>
<span data-ttu-id="e8a25-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8a25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8a25-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8a25-110">Permission type</span></span>      | <span data-ttu-id="e8a25-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8a25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8a25-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8a25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8a25-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a25-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8a25-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8a25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a25-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8a25-115">Not supported.</span></span>    |
|<span data-ttu-id="e8a25-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8a25-116">Application</span></span> | <span data-ttu-id="e8a25-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a25-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="e8a25-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e8a25-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e8a25-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="e8a25-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e8a25-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8a25-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e8a25-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8a25-121">Request headers</span></span>
| <span data-ttu-id="e8a25-122">标头</span><span class="sxs-lookup"><span data-stu-id="e8a25-122">Header</span></span>       | <span data-ttu-id="e8a25-123">值</span><span class="sxs-lookup"><span data-stu-id="e8a25-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8a25-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8a25-124">Authorization</span></span>  | <span data-ttu-id="e8a25-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8a25-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8a25-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8a25-127">Request body</span></span>
<span data-ttu-id="e8a25-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8a25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a25-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8a25-129">Response</span></span>

<span data-ttu-id="e8a25-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e8a25-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8a25-132">示例</span><span class="sxs-lookup"><span data-stu-id="e8a25-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8a25-133">请求</span><span class="sxs-lookup"><span data-stu-id="e8a25-133">Request</span></span>
<span data-ttu-id="e8a25-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8a25-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="e8a25-135">响应</span><span class="sxs-lookup"><span data-stu-id="e8a25-135">Response</span></span>

<span data-ttu-id="e8a25-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8a25-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
