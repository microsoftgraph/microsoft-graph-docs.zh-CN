---
title: 删除用户-Microsoft Graph API
description: 介绍 Microsoft Graph API (REST) 的用户资源 (实体) 的 delete 方法。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f7f8ed5b11930865d88ed7f01530c052c3e63738
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253790"
---
# <a name="delete-a-user"></a><span data-ttu-id="aac53-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="aac53-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aac53-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="aac53-104">Delete user.</span></span>  

<span data-ttu-id="aac53-105">删除后, 用户资源将移至临时容器, 并可在30天内恢复。</span><span class="sxs-lookup"><span data-stu-id="aac53-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="aac53-106">之后, 它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="aac53-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="aac53-107">若要了解详细信息, 请参阅[deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="aac53-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aac53-108">权限</span><span class="sxs-lookup"><span data-stu-id="aac53-108">Permissions</span></span>

<span data-ttu-id="aac53-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aac53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac53-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aac53-111">Permission type</span></span>      | <span data-ttu-id="aac53-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aac53-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac53-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aac53-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aac53-114">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aac53-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aac53-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aac53-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac53-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aac53-116">Not supported.</span></span>    |
|<span data-ttu-id="aac53-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aac53-117">Application</span></span> | <span data-ttu-id="aac53-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac53-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aac53-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aac53-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="aac53-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aac53-120">Request headers</span></span>

| <span data-ttu-id="aac53-121">标头</span><span class="sxs-lookup"><span data-stu-id="aac53-121">Header</span></span>       | <span data-ttu-id="aac53-122">值</span><span class="sxs-lookup"><span data-stu-id="aac53-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="aac53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac53-123">Authorization</span></span>  | <span data-ttu-id="aac53-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aac53-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aac53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aac53-126">Request body</span></span>

<span data-ttu-id="aac53-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aac53-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac53-128">响应</span><span class="sxs-lookup"><span data-stu-id="aac53-128">Response</span></span>

<span data-ttu-id="aac53-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aac53-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac53-131">示例</span><span class="sxs-lookup"><span data-stu-id="aac53-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac53-132">请求</span><span class="sxs-lookup"><span data-stu-id="aac53-132">Request</span></span>

<span data-ttu-id="aac53-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aac53-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
### <a name="response"></a><span data-ttu-id="aac53-134">响应</span><span class="sxs-lookup"><span data-stu-id="aac53-134">Response</span></span>

<span data-ttu-id="aac53-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aac53-135">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
