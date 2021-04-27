---
title: 删除音频路由组
description: 删除指定的音频路由组。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: de1ac6aa2a296cf95fddb33c075f52ce57da0d81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048020"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="3ce7a-103">删除音频路由组</span><span class="sxs-lookup"><span data-stu-id="3ce7a-103">Delete audio routing group</span></span>

<span data-ttu-id="3ce7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ce7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce7a-105">删除指定的 [audioRoutingGroup](../resources/audioroutinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-105">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ce7a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ce7a-106">Permissions</span></span>
<span data-ttu-id="3ce7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ce7a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ce7a-109">Permission type</span></span> | <span data-ttu-id="3ce7a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ce7a-110">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="3ce7a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ce7a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ce7a-112">不支持</span><span class="sxs-lookup"><span data-stu-id="3ce7a-112">Not Supported</span></span>        |
| <span data-ttu-id="3ce7a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ce7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ce7a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="3ce7a-114">Not Supported</span></span>        |
| <span data-ttu-id="3ce7a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ce7a-115">Application</span></span>     | <span data-ttu-id="3ce7a-116">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="3ce7a-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ce7a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ce7a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /communications/calls/{id}/audioRoutingGroups/{id}
```
> <span data-ttu-id="3ce7a-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3ce7a-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ce7a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ce7a-120">Request headers</span></span>
| <span data-ttu-id="3ce7a-121">名称</span><span class="sxs-lookup"><span data-stu-id="3ce7a-121">Name</span></span>          | <span data-ttu-id="3ce7a-122">说明</span><span class="sxs-lookup"><span data-stu-id="3ce7a-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3ce7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce7a-123">Authorization</span></span> | <span data-ttu-id="3ce7a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ce7a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ce7a-126">Request body</span></span>
<span data-ttu-id="3ce7a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ce7a-128">响应</span><span class="sxs-lookup"><span data-stu-id="3ce7a-128">Response</span></span>
<span data-ttu-id="3ce7a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce7a-131">示例</span><span class="sxs-lookup"><span data-stu-id="3ce7a-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ce7a-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ce7a-132">Request</span></span>
<span data-ttu-id="3ce7a-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ce7a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce7a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/audioRoutingGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="3ce7a-135">C#</span><span class="sxs-lookup"><span data-stu-id="3ce7a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-audioroutinggroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ce7a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ce7a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-audioroutinggroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ce7a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ce7a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-audioroutinggroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ce7a-138">Java</span><span class="sxs-lookup"><span data-stu-id="3ce7a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-audioroutinggroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3ce7a-139">响应</span><span class="sxs-lookup"><span data-stu-id="3ce7a-139">Response</span></span>

> <span data-ttu-id="3ce7a-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ce7a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


