---
title: 删除组-Microsoft Graph API
description: 删除组资源。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d09a5c4e214e8f2edee31162f7a2af4b949f0b42
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895585"
---
# <a name="delete-group"></a><span data-ttu-id="c5259-103">删除组</span><span class="sxs-lookup"><span data-stu-id="c5259-103">Delete group</span></span>

<span data-ttu-id="c5259-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5259-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5259-105">删除组。</span><span class="sxs-lookup"><span data-stu-id="c5259-105">Delete group.</span></span>  

<span data-ttu-id="c5259-106">删除后，Microsoft 365 组将移至临时容器，并可在30天内恢复。</span><span class="sxs-lookup"><span data-stu-id="c5259-106">When deleted, Microsoft 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="c5259-107">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="c5259-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="c5259-108">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="c5259-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="c5259-109">这仅适用于 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="c5259-109">This applies only to Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5259-110">权限</span><span class="sxs-lookup"><span data-stu-id="c5259-110">Permissions</span></span>

<span data-ttu-id="c5259-111">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c5259-111">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c5259-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5259-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5259-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5259-113">Permission type</span></span>      | <span data-ttu-id="c5259-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5259-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5259-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5259-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c5259-116">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5259-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="c5259-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5259-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5259-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5259-118">Not supported.</span></span>    |
|<span data-ttu-id="c5259-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5259-119">Application</span></span> | <span data-ttu-id="c5259-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5259-120">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5259-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5259-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c5259-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5259-122">Request headers</span></span>

| <span data-ttu-id="c5259-123">名称</span><span class="sxs-lookup"><span data-stu-id="c5259-123">Name</span></span>       | <span data-ttu-id="c5259-124">类型</span><span class="sxs-lookup"><span data-stu-id="c5259-124">Type</span></span> | <span data-ttu-id="c5259-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5259-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5259-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5259-126">Authorization</span></span>  | <span data-ttu-id="c5259-127">string</span><span class="sxs-lookup"><span data-stu-id="c5259-127">string</span></span>  | <span data-ttu-id="c5259-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c5259-128">Bearer {token}.</span></span> <span data-ttu-id="c5259-129">Required.</span><span class="sxs-lookup"><span data-stu-id="c5259-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5259-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5259-130">Request body</span></span>

<span data-ttu-id="c5259-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5259-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5259-132">响应</span><span class="sxs-lookup"><span data-stu-id="c5259-132">Response</span></span>

<span data-ttu-id="c5259-133">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="c5259-133">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="c5259-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="c5259-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5259-135">示例</span><span class="sxs-lookup"><span data-stu-id="c5259-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5259-136">请求</span><span class="sxs-lookup"><span data-stu-id="c5259-136">Request</span></span>

<span data-ttu-id="c5259-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5259-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5259-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5259-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
# <a name="c"></a>[<span data-ttu-id="c5259-139">C#</span><span class="sxs-lookup"><span data-stu-id="c5259-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5259-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5259-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5259-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5259-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5259-142">Java</span><span class="sxs-lookup"><span data-stu-id="c5259-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5259-143">响应</span><span class="sxs-lookup"><span data-stu-id="c5259-143">Response</span></span>

<span data-ttu-id="c5259-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5259-144">The following is an example of the response.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
