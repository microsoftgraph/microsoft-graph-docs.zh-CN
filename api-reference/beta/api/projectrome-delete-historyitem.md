---
title: 删除 historyItem
description: 删除现有用户活动的现有历史记录项。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 42112754e7ce3388cb4e45eb1cf82426cdedbbc1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810011"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="5aaf8-103">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="5aaf8-103">Delete a historyItem</span></span>

<span data-ttu-id="5aaf8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aaf8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aaf8-105">删除现有用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-105">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aaf8-106">权限</span><span class="sxs-lookup"><span data-stu-id="5aaf8-106">Permissions</span></span>

<span data-ttu-id="5aaf8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5aaf8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5aaf8-109">Permission type</span></span>      | <span data-ttu-id="5aaf8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5aaf8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5aaf8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5aaf8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5aaf8-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5aaf8-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5aaf8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5aaf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aaf8-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5aaf8-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5aaf8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5aaf8-115">Application</span></span> | <span data-ttu-id="5aaf8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5aaf8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5aaf8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5aaf8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5aaf8-118">Request headers</span></span>

|<span data-ttu-id="5aaf8-119">名称</span><span class="sxs-lookup"><span data-stu-id="5aaf8-119">Name</span></span> | <span data-ttu-id="5aaf8-120">类型</span><span class="sxs-lookup"><span data-stu-id="5aaf8-120">Type</span></span> | <span data-ttu-id="5aaf8-121">说明</span><span class="sxs-lookup"><span data-stu-id="5aaf8-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5aaf8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aaf8-122">Authorization</span></span> | <span data-ttu-id="5aaf8-123">string</span><span class="sxs-lookup"><span data-stu-id="5aaf8-123">string</span></span> | <span data-ttu-id="5aaf8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aaf8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5aaf8-126">Request body</span></span>

<span data-ttu-id="5aaf8-127">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="5aaf8-128">响应</span><span class="sxs-lookup"><span data-stu-id="5aaf8-128">Response</span></span>

<span data-ttu-id="5aaf8-129">如果成功，此方法在 `204 No Content` 历史记录项被删除时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-129">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="5aaf8-130">示例</span><span class="sxs-lookup"><span data-stu-id="5aaf8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5aaf8-131">请求</span><span class="sxs-lookup"><span data-stu-id="5aaf8-131">Request</span></span>

<span data-ttu-id="5aaf8-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5aaf8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aaf8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```
# <a name="objective-c"></a>[<span data-ttu-id="5aaf8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aaf8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5aaf8-135">响应</span><span class="sxs-lookup"><span data-stu-id="5aaf8-135">Response</span></span>

<span data-ttu-id="5aaf8-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5aaf8-136">Here is an example of the response.</span></span>

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
