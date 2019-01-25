---
title: 删除音频路由组
description: 删除指定的音频路由组。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0c0e5c0cd58c867f7c69a3ac5d4f99a11af223ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511441"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="680fe-103">删除音频路由组</span><span class="sxs-lookup"><span data-stu-id="680fe-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="680fe-104">删除指定的[audioRoutingGroup](../resources/audioroutinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="680fe-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="680fe-105">权限</span><span class="sxs-lookup"><span data-stu-id="680fe-105">Permissions</span></span>
<span data-ttu-id="680fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="680fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="680fe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="680fe-108">Permission type</span></span> | <span data-ttu-id="680fe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="680fe-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="680fe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="680fe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="680fe-111">不支持</span><span class="sxs-lookup"><span data-stu-id="680fe-111">Not Supported</span></span>        |
| <span data-ttu-id="680fe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="680fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="680fe-113">不支持</span><span class="sxs-lookup"><span data-stu-id="680fe-113">Not Supported</span></span>        |
| <span data-ttu-id="680fe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="680fe-114">Application</span></span>     | <span data-ttu-id="680fe-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="680fe-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="680fe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="680fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="680fe-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="680fe-117">Request headers</span></span>
| <span data-ttu-id="680fe-118">名称</span><span class="sxs-lookup"><span data-stu-id="680fe-118">Name</span></span>          | <span data-ttu-id="680fe-119">说明</span><span class="sxs-lookup"><span data-stu-id="680fe-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="680fe-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="680fe-120">Authorization</span></span> | <span data-ttu-id="680fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="680fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="680fe-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="680fe-123">Request body</span></span>
<span data-ttu-id="680fe-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="680fe-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="680fe-125">响应</span><span class="sxs-lookup"><span data-stu-id="680fe-125">Response</span></span>
<span data-ttu-id="680fe-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="680fe-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="680fe-128">示例</span><span class="sxs-lookup"><span data-stu-id="680fe-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="680fe-129">请求</span><span class="sxs-lookup"><span data-stu-id="680fe-129">Request</span></span>
<span data-ttu-id="680fe-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="680fe-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="680fe-131">响应</span><span class="sxs-lookup"><span data-stu-id="680fe-131">Response</span></span>

> <span data-ttu-id="680fe-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="680fe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
