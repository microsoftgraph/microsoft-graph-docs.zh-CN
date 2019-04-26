---
title: 删除 timeOff
description: 从计划中删除 timeOff 实例。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 361c850de6a1171e753da6bb7266e994df6e35ac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330081"
---
# <a name="delete-timeoff"></a><span data-ttu-id="a3698-103">删除 timeOff</span><span class="sxs-lookup"><span data-stu-id="a3698-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3698-104">从[计划](../resources/schedule.md)中删除[timeOff](../resources/timeoff.md)实例。</span><span class="sxs-lookup"><span data-stu-id="a3698-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a3698-105">权限</span><span class="sxs-lookup"><span data-stu-id="a3698-105">Permissions</span></span>

<span data-ttu-id="a3698-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3698-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3698-108">Permission type</span></span>      | <span data-ttu-id="a3698-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3698-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3698-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3698-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3698-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3698-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3698-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3698-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3698-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3698-113">Not supported.</span></span>    |
|<span data-ttu-id="a3698-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3698-114">Application</span></span> | <span data-ttu-id="a3698-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3698-115">Not supported.</span></span> |

> <span data-ttu-id="a3698-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a3698-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a3698-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="a3698-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3698-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3698-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="a3698-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3698-119">Request headers</span></span>

| <span data-ttu-id="a3698-120">标头</span><span class="sxs-lookup"><span data-stu-id="a3698-120">Header</span></span>       | <span data-ttu-id="a3698-121">值</span><span class="sxs-lookup"><span data-stu-id="a3698-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3698-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3698-122">Authorization</span></span>  | <span data-ttu-id="a3698-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3698-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3698-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3698-125">Content-Type</span></span>  | <span data-ttu-id="a3698-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3698-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3698-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3698-127">Request body</span></span>
<span data-ttu-id="a3698-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3698-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3698-129">响应</span><span class="sxs-lookup"><span data-stu-id="a3698-129">Response</span></span>

<span data-ttu-id="a3698-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a3698-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3698-132">示例</span><span class="sxs-lookup"><span data-stu-id="a3698-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a3698-133">请求</span><span class="sxs-lookup"><span data-stu-id="a3698-133">Request</span></span>

<span data-ttu-id="a3698-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3698-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="a3698-135">响应</span><span class="sxs-lookup"><span data-stu-id="a3698-135">Response</span></span>

<span data-ttu-id="a3698-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3698-136">The following is an example of the response.</span></span> 

><span data-ttu-id="a3698-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3698-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
