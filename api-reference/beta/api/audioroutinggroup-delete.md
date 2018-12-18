---
title: 删除音频路由组
description: 删除指定的 audioRoutingGroup。
author: VinodRavichandran
ms.openlocfilehash: 025498e1ceb6178ede4c7ca938c7b0d3d05a80ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323938"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="06182-103">删除音频路由组</span><span class="sxs-lookup"><span data-stu-id="06182-103">Delete audio routing group</span></span>

> <span data-ttu-id="06182-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06182-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06182-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06182-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06182-106">删除指定的[audioRoutingGroup](../resources/audioroutinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="06182-106">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06182-107">权限</span><span class="sxs-lookup"><span data-stu-id="06182-107">Permissions</span></span>
<span data-ttu-id="06182-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06182-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06182-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="06182-110">Permission type</span></span> | <span data-ttu-id="06182-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06182-111">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="06182-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06182-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="06182-113">不支持</span><span class="sxs-lookup"><span data-stu-id="06182-113">Not Supported</span></span>        |
| <span data-ttu-id="06182-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06182-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06182-115">不支持</span><span class="sxs-lookup"><span data-stu-id="06182-115">Not Supported</span></span>        |
| <span data-ttu-id="06182-116">Application</span><span class="sxs-lookup"><span data-stu-id="06182-116">Application</span></span>     | <span data-ttu-id="06182-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="06182-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06182-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06182-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="06182-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06182-119">Request headers</span></span>
| <span data-ttu-id="06182-120">Name</span><span class="sxs-lookup"><span data-stu-id="06182-120">Name</span></span>          | <span data-ttu-id="06182-121">说明</span><span class="sxs-lookup"><span data-stu-id="06182-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="06182-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06182-122">Authorization</span></span> | <span data-ttu-id="06182-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06182-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06182-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="06182-125">Request body</span></span>
<span data-ttu-id="06182-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06182-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06182-127">响应</span><span class="sxs-lookup"><span data-stu-id="06182-127">Response</span></span>
<span data-ttu-id="06182-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="06182-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06182-130">示例</span><span class="sxs-lookup"><span data-stu-id="06182-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="06182-131">请求</span><span class="sxs-lookup"><span data-stu-id="06182-131">Request</span></span>
<span data-ttu-id="06182-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="06182-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="06182-133">响应</span><span class="sxs-lookup"><span data-stu-id="06182-133">Response</span></span>

> <span data-ttu-id="06182-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="06182-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
