---
title: 删除 historyItem
description: 删除现有用户活动的现有历史记录项。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5a3cac83c220a8fa15a3d5277af319117bd7c927
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264062"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="1e7c1-103">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="1e7c1-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e7c1-104">删除现有用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e7c1-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e7c1-105">Permissions</span></span>

<span data-ttu-id="1e7c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e7c1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e7c1-108">Permission type</span></span>      | <span data-ttu-id="1e7c1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e7c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e7c1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e7c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e7c1-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1e7c1-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1e7c1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e7c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e7c1-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1e7c1-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1e7c1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e7c1-114">Application</span></span> | <span data-ttu-id="1e7c1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e7c1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e7c1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e7c1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e7c1-117">Request headers</span></span>

|<span data-ttu-id="1e7c1-118">名称</span><span class="sxs-lookup"><span data-stu-id="1e7c1-118">Name</span></span> | <span data-ttu-id="1e7c1-119">类型</span><span class="sxs-lookup"><span data-stu-id="1e7c1-119">Type</span></span> | <span data-ttu-id="1e7c1-120">说明</span><span class="sxs-lookup"><span data-stu-id="1e7c1-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1e7c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e7c1-121">Authorization</span></span> | <span data-ttu-id="1e7c1-122">string</span><span class="sxs-lookup"><span data-stu-id="1e7c1-122">string</span></span> | <span data-ttu-id="1e7c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e7c1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e7c1-125">Request body</span></span>

<span data-ttu-id="1e7c1-126">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="1e7c1-127">响应</span><span class="sxs-lookup"><span data-stu-id="1e7c1-127">Response</span></span>

<span data-ttu-id="1e7c1-128">如果成功, 此方法在历史`204 No Content`记录项被删除时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="1e7c1-129">示例</span><span class="sxs-lookup"><span data-stu-id="1e7c1-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1e7c1-130">请求</span><span class="sxs-lookup"><span data-stu-id="1e7c1-130">Request</span></span>

<span data-ttu-id="1e7c1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="1e7c1-132">响应</span><span class="sxs-lookup"><span data-stu-id="1e7c1-132">Response</span></span>

<span data-ttu-id="1e7c1-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1e7c1-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1e7c1-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1e7c1-134">SDK sample code</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1e7c1-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e7c1-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_historyItem-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)"
  ]
}
-->
