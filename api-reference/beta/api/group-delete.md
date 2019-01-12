---
title: 删除组
description: 删除组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 75b5d03cb5bce93966efc1495fd4284060580189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916451"
---
# <a name="delete-group"></a><span data-ttu-id="8e23a-103">删除组</span><span class="sxs-lookup"><span data-stu-id="8e23a-103">Delete group</span></span>

> <span data-ttu-id="8e23a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e23a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e23a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e23a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e23a-106">删除组。</span><span class="sxs-lookup"><span data-stu-id="8e23a-106">Deletes a group.</span></span>

<span data-ttu-id="8e23a-107">删除组后，项目添加到[已删除项目](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="8e23a-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="8e23a-108">组将已删除的项目中保持最多 30 天。</span><span class="sxs-lookup"><span data-stu-id="8e23a-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="8e23a-109">组可以完全从还原已删除项目在 30 天。</span><span class="sxs-lookup"><span data-stu-id="8e23a-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="8e23a-110">30 天后删除的项目被永久删除。</span><span class="sxs-lookup"><span data-stu-id="8e23a-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e23a-111">权限</span><span class="sxs-lookup"><span data-stu-id="8e23a-111">Permissions</span></span>
<span data-ttu-id="8e23a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e23a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e23a-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e23a-114">Permission type</span></span>      | <span data-ttu-id="8e23a-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e23a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e23a-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e23a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8e23a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e23a-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e23a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e23a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e23a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e23a-119">Not supported.</span></span>    |
|<span data-ttu-id="8e23a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e23a-120">Application</span></span> | <span data-ttu-id="8e23a-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e23a-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e23a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e23a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8e23a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e23a-123">Request headers</span></span>
| <span data-ttu-id="8e23a-124">名称</span><span class="sxs-lookup"><span data-stu-id="8e23a-124">Name</span></span>       | <span data-ttu-id="8e23a-125">类型</span><span class="sxs-lookup"><span data-stu-id="8e23a-125">Type</span></span> | <span data-ttu-id="8e23a-126">说明</span><span class="sxs-lookup"><span data-stu-id="8e23a-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e23a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e23a-127">Authorization</span></span>  | <span data-ttu-id="8e23a-128">string</span><span class="sxs-lookup"><span data-stu-id="8e23a-128">string</span></span>  | <span data-ttu-id="8e23a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e23a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e23a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e23a-131">Request body</span></span>
<span data-ttu-id="8e23a-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e23a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e23a-133">响应</span><span class="sxs-lookup"><span data-stu-id="8e23a-133">Response</span></span>
<span data-ttu-id="8e23a-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8e23a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e23a-136">示例</span><span class="sxs-lookup"><span data-stu-id="8e23a-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8e23a-137">请求</span><span class="sxs-lookup"><span data-stu-id="8e23a-137">Request</span></span>
<span data-ttu-id="8e23a-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e23a-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="8e23a-139">响应</span><span class="sxs-lookup"><span data-stu-id="8e23a-139">Response</span></span>
<span data-ttu-id="8e23a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e23a-140">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
