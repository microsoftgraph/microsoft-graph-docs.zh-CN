---
title: 从频道中删除选项卡
description: '从团队中的指定通道中删除 (unpins) 选项卡。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3dbba4b8996a86e8ff71d0dd115b0a00362e103f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027207"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="53c99-103">从频道中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="53c99-103">Delete tab from channel</span></span>



<span data-ttu-id="53c99-104">从[团队](../resources/team.md)中的指定[通道](../resources/channel.md)中删除 (unpins) 选项卡。</span><span class="sxs-lookup"><span data-stu-id="53c99-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="53c99-105">权限</span><span class="sxs-lookup"><span data-stu-id="53c99-105">Permissions</span></span>
<span data-ttu-id="53c99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c99-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53c99-108">Permission type</span></span>      | <span data-ttu-id="53c99-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53c99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53c99-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53c99-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53c99-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c99-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="53c99-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53c99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53c99-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="53c99-113">Not supported.</span></span>    |
|<span data-ttu-id="53c99-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53c99-114">Application</span></span> | <span data-ttu-id="53c99-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c99-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="53c99-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="53c99-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="53c99-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="53c99-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="53c99-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53c99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53c99-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53c99-119">Request headers</span></span>
| <span data-ttu-id="53c99-120">标头</span><span class="sxs-lookup"><span data-stu-id="53c99-120">Header</span></span>       | <span data-ttu-id="53c99-121">值</span><span class="sxs-lookup"><span data-stu-id="53c99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53c99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53c99-122">Authorization</span></span>  | <span data-ttu-id="53c99-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53c99-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53c99-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53c99-125">Request body</span></span>
<span data-ttu-id="53c99-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53c99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53c99-127">响应</span><span class="sxs-lookup"><span data-stu-id="53c99-127">Response</span></span>

<span data-ttu-id="53c99-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="53c99-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c99-130">示例</span><span class="sxs-lookup"><span data-stu-id="53c99-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="53c99-131">请求</span><span class="sxs-lookup"><span data-stu-id="53c99-131">Request</span></span>
<span data-ttu-id="53c99-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53c99-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="53c99-133">响应</span><span class="sxs-lookup"><span data-stu-id="53c99-133">Response</span></span>
<span data-ttu-id="53c99-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53c99-134">The following is an example of the response.</span></span> <span data-ttu-id="53c99-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53c99-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="53c99-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53c99-136">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
