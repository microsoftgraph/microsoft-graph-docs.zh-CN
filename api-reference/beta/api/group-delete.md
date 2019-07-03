---
title: 删除组-Microsoft Graph API
description: 介绍 Microsoft Graph API (REST) 的组资源 (实体) 的 delete 方法。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a0a7ba7c49714ac685920b6ee70f9e71df7dfa92
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440615"
---
# <a name="delete-group"></a><span data-ttu-id="17d65-103">删除组</span><span class="sxs-lookup"><span data-stu-id="17d65-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17d65-104">删除组。</span><span class="sxs-lookup"><span data-stu-id="17d65-104">Deletes a group.</span></span>  

<span data-ttu-id="17d65-105">删除后, Office 365 组将移至临时容器, 并可在30天内恢复。</span><span class="sxs-lookup"><span data-stu-id="17d65-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="17d65-106">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="17d65-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="17d65-107">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="17d65-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="17d65-108">这仅适用于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="17d65-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="17d65-109">权限</span><span class="sxs-lookup"><span data-stu-id="17d65-109">Permissions</span></span>

<span data-ttu-id="17d65-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17d65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17d65-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="17d65-112">Permission type</span></span>      | <span data-ttu-id="17d65-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17d65-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17d65-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17d65-114">Delegated (work or school account)</span></span> | <span data-ttu-id="17d65-115">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17d65-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="17d65-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17d65-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17d65-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="17d65-117">Not supported.</span></span>    |
|<span data-ttu-id="17d65-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="17d65-118">Application</span></span> | <span data-ttu-id="17d65-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d65-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17d65-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17d65-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="17d65-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="17d65-121">Request headers</span></span>

| <span data-ttu-id="17d65-122">名称</span><span class="sxs-lookup"><span data-stu-id="17d65-122">Name</span></span>       | <span data-ttu-id="17d65-123">类型</span><span class="sxs-lookup"><span data-stu-id="17d65-123">Type</span></span> | <span data-ttu-id="17d65-124">说明</span><span class="sxs-lookup"><span data-stu-id="17d65-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17d65-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="17d65-125">Authorization</span></span>  | <span data-ttu-id="17d65-126">string</span><span class="sxs-lookup"><span data-stu-id="17d65-126">string</span></span>  | <span data-ttu-id="17d65-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17d65-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17d65-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="17d65-129">Request body</span></span>

<span data-ttu-id="17d65-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17d65-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17d65-131">响应</span><span class="sxs-lookup"><span data-stu-id="17d65-131">Response</span></span>

<span data-ttu-id="17d65-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="17d65-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17d65-134">示例</span><span class="sxs-lookup"><span data-stu-id="17d65-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="17d65-135">请求</span><span class="sxs-lookup"><span data-stu-id="17d65-135">Request</span></span>

<span data-ttu-id="17d65-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17d65-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17d65-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="17d65-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17d65-138">C#</span><span class="sxs-lookup"><span data-stu-id="17d65-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17d65-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="17d65-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17d65-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="17d65-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17d65-141">响应</span><span class="sxs-lookup"><span data-stu-id="17d65-141">Response</span></span>

<span data-ttu-id="17d65-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17d65-142">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
