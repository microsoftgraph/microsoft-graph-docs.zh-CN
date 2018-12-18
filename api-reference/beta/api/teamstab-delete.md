---
title: 从通道删除选项卡
description: '删除 （取消锁定） 从指定的通道团队中的一个选项卡。 '
author: nkramer
ms.openlocfilehash: 7d8465f650d63f22625c1da2c56b3de4e065374b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349285"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="2b639-103">从通道删除选项卡</span><span class="sxs-lookup"><span data-stu-id="2b639-103">Delete tab from channel</span></span>

> <span data-ttu-id="2b639-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2b639-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b639-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b639-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b639-106">删除 （取消锁定） 从指定的[频道](../resources/channel.md)[团队](../resources/team.md)中的一个选项卡。</span><span class="sxs-lookup"><span data-stu-id="2b639-106">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2b639-107">权限</span><span class="sxs-lookup"><span data-stu-id="2b639-107">Permissions</span></span>
<span data-ttu-id="2b639-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b639-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b639-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b639-110">Permission type</span></span>      | <span data-ttu-id="2b639-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b639-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b639-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b639-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b639-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b639-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b639-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b639-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b639-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b639-115">Not supported.</span></span>    |
|<span data-ttu-id="2b639-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b639-116">Application</span></span> | <span data-ttu-id="2b639-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b639-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="2b639-118">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="2b639-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2b639-119">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="2b639-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b639-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b639-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b639-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b639-121">Request headers</span></span>
| <span data-ttu-id="2b639-122">标头</span><span class="sxs-lookup"><span data-stu-id="2b639-122">Header</span></span>       | <span data-ttu-id="2b639-123">值</span><span class="sxs-lookup"><span data-stu-id="2b639-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b639-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b639-124">Authorization</span></span>  | <span data-ttu-id="2b639-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b639-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b639-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b639-127">Request body</span></span>
<span data-ttu-id="2b639-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b639-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b639-129">响应</span><span class="sxs-lookup"><span data-stu-id="2b639-129">Response</span></span>

<span data-ttu-id="2b639-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2b639-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b639-132">示例</span><span class="sxs-lookup"><span data-stu-id="2b639-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2b639-133">请求</span><span class="sxs-lookup"><span data-stu-id="2b639-133">Request</span></span>
<span data-ttu-id="2b639-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2b639-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="2b639-135">响应</span><span class="sxs-lookup"><span data-stu-id="2b639-135">Response</span></span>
<span data-ttu-id="2b639-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b639-136">The following is an example of the response.</span></span> <span data-ttu-id="2b639-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2b639-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2b639-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b639-138">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
