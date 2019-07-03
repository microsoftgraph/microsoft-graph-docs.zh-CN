---
title: 删除音频路由组
description: 删除指定的音频路由组。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3034b94e351e12a5427f33cd0707632307ac928a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439425"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="2b5bd-103">删除音频路由组</span><span class="sxs-lookup"><span data-stu-id="2b5bd-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b5bd-104">删除指定的[audioRoutingGroup](../resources/audioroutinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b5bd-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b5bd-105">Permissions</span></span>
<span data-ttu-id="2b5bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b5bd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b5bd-108">Permission type</span></span> | <span data-ttu-id="2b5bd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b5bd-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="2b5bd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b5bd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b5bd-111">不支持</span><span class="sxs-lookup"><span data-stu-id="2b5bd-111">Not Supported</span></span>        |
| <span data-ttu-id="2b5bd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b5bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b5bd-113">不支持</span><span class="sxs-lookup"><span data-stu-id="2b5bd-113">Not Supported</span></span>        |
| <span data-ttu-id="2b5bd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b5bd-114">Application</span></span>     | <span data-ttu-id="2b5bd-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="2b5bd-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b5bd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b5bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b5bd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b5bd-117">Request headers</span></span>
| <span data-ttu-id="2b5bd-118">名称</span><span class="sxs-lookup"><span data-stu-id="2b5bd-118">Name</span></span>          | <span data-ttu-id="2b5bd-119">说明</span><span class="sxs-lookup"><span data-stu-id="2b5bd-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2b5bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b5bd-120">Authorization</span></span> | <span data-ttu-id="2b5bd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b5bd-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b5bd-123">Request body</span></span>
<span data-ttu-id="2b5bd-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b5bd-125">响应</span><span class="sxs-lookup"><span data-stu-id="2b5bd-125">Response</span></span>
<span data-ttu-id="2b5bd-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b5bd-128">示例</span><span class="sxs-lookup"><span data-stu-id="2b5bd-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b5bd-129">请求</span><span class="sxs-lookup"><span data-stu-id="2b5bd-129">Request</span></span>
<span data-ttu-id="2b5bd-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2b5bd-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2b5bd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b5bd-132">C#</span><span class="sxs-lookup"><span data-stu-id="2b5bd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b5bd-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b5bd-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b5bd-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="2b5bd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b5bd-135">响应</span><span class="sxs-lookup"><span data-stu-id="2b5bd-135">Response</span></span>

> <span data-ttu-id="2b5bd-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2b5bd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
