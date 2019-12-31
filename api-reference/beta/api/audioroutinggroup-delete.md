---
title: 删除音频路由组
description: 删除指定的音频路由组。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7f89c223c7e45ccaa5a25fe7bbdd7a53f529880f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911818"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="8520c-103">删除音频路由组</span><span class="sxs-lookup"><span data-stu-id="8520c-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8520c-104">删除指定的[audioRoutingGroup](../resources/audioroutinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="8520c-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8520c-105">权限</span><span class="sxs-lookup"><span data-stu-id="8520c-105">Permissions</span></span>
<span data-ttu-id="8520c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8520c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8520c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8520c-108">Permission type</span></span> | <span data-ttu-id="8520c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8520c-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="8520c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8520c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8520c-111">不支持</span><span class="sxs-lookup"><span data-stu-id="8520c-111">Not Supported</span></span>        |
| <span data-ttu-id="8520c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8520c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8520c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8520c-113">Not Supported</span></span>        |
| <span data-ttu-id="8520c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8520c-114">Application</span></span>     | <span data-ttu-id="8520c-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="8520c-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8520c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8520c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="8520c-117">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="8520c-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8520c-118">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="8520c-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8520c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8520c-119">Request headers</span></span>
| <span data-ttu-id="8520c-120">名称</span><span class="sxs-lookup"><span data-stu-id="8520c-120">Name</span></span>          | <span data-ttu-id="8520c-121">说明</span><span class="sxs-lookup"><span data-stu-id="8520c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8520c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8520c-122">Authorization</span></span> | <span data-ttu-id="8520c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8520c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8520c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8520c-125">Request body</span></span>
<span data-ttu-id="8520c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8520c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8520c-127">响应</span><span class="sxs-lookup"><span data-stu-id="8520c-127">Response</span></span>
<span data-ttu-id="8520c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8520c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8520c-130">示例</span><span class="sxs-lookup"><span data-stu-id="8520c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8520c-131">请求</span><span class="sxs-lookup"><span data-stu-id="8520c-131">Request</span></span>
<span data-ttu-id="8520c-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8520c-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8520c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8520c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8520c-134">C#</span><span class="sxs-lookup"><span data-stu-id="8520c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8520c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8520c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8520c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8520c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8520c-137">响应</span><span class="sxs-lookup"><span data-stu-id="8520c-137">Response</span></span>

> <span data-ttu-id="8520c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8520c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
