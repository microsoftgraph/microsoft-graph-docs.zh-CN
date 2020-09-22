---
title: 删除 historyItem
description: 删除现有用户活动的现有历史记录项。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 1fa3b1863445caa5ce7a953a98d12310b4abeec9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017302"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="ce772-103">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="ce772-103">Delete a historyItem</span></span>

<span data-ttu-id="ce772-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce772-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce772-105">删除现有用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="ce772-105">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce772-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce772-106">Permissions</span></span>

<span data-ttu-id="ce772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ce772-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce772-109">Permission type</span></span>      | <span data-ttu-id="ce772-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce772-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce772-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce772-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ce772-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ce772-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ce772-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce772-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce772-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ce772-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ce772-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce772-115">Application</span></span> | <span data-ttu-id="ce772-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce772-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce772-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce772-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ce772-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce772-118">Request headers</span></span>

|<span data-ttu-id="ce772-119">名称</span><span class="sxs-lookup"><span data-stu-id="ce772-119">Name</span></span> | <span data-ttu-id="ce772-120">类型</span><span class="sxs-lookup"><span data-stu-id="ce772-120">Type</span></span> | <span data-ttu-id="ce772-121">说明</span><span class="sxs-lookup"><span data-stu-id="ce772-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ce772-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce772-122">Authorization</span></span> | <span data-ttu-id="ce772-123">string</span><span class="sxs-lookup"><span data-stu-id="ce772-123">string</span></span> | <span data-ttu-id="ce772-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce772-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce772-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce772-126">Request body</span></span>

<span data-ttu-id="ce772-127">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce772-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="ce772-128">响应</span><span class="sxs-lookup"><span data-stu-id="ce772-128">Response</span></span>

<span data-ttu-id="ce772-129">如果成功，此方法在 `204 No Content` 历史记录项被删除时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="ce772-129">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="ce772-130">示例</span><span class="sxs-lookup"><span data-stu-id="ce772-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ce772-131">请求</span><span class="sxs-lookup"><span data-stu-id="ce772-131">Request</span></span>

<span data-ttu-id="ce772-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce772-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce772-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce772-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```
# <a name="objective-c"></a>[<span data-ttu-id="ce772-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce772-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ce772-135">响应</span><span class="sxs-lookup"><span data-stu-id="ce772-135">Response</span></span>

<span data-ttu-id="ce772-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ce772-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


