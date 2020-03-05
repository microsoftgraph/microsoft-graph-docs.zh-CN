---
title: 删除 educationalActivity
description: 从用户配置文件中删除 educationalActivity 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b1c4a5069f192a481b9f4814115e3d6fcee6fc55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427898"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="1a478-103">删除 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="1a478-103">Delete educationalActivity</span></span>

<span data-ttu-id="1a478-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1a478-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a478-105">从用户的[配置文件](../resources/profile.md)中删除[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a478-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a478-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a478-106">Permissions</span></span>

<span data-ttu-id="1a478-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a478-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a478-109">Permission type</span></span>                        | <span data-ttu-id="1a478-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a478-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a478-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a478-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a478-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="1a478-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1a478-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a478-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a478-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="1a478-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1a478-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a478-115">Application</span></span>                            | <span data-ttu-id="1a478-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a478-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1a478-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a478-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="1a478-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a478-118">Request headers</span></span>

| <span data-ttu-id="1a478-119">名称</span><span class="sxs-lookup"><span data-stu-id="1a478-119">Name</span></span>           |<span data-ttu-id="1a478-120">说明</span><span class="sxs-lookup"><span data-stu-id="1a478-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1a478-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a478-121">Authorization</span></span>  | <span data-ttu-id="1a478-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a478-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="1a478-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a478-124">Request body</span></span>

<span data-ttu-id="1a478-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a478-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a478-126">响应</span><span class="sxs-lookup"><span data-stu-id="1a478-126">Response</span></span>

<span data-ttu-id="1a478-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1a478-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a478-129">示例</span><span class="sxs-lookup"><span data-stu-id="1a478-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a478-130">请求</span><span class="sxs-lookup"><span data-stu-id="1a478-130">Request</span></span>

<span data-ttu-id="1a478-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a478-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/educationalActivities/{id}
```

### <a name="response"></a><span data-ttu-id="1a478-132">响应</span><span class="sxs-lookup"><span data-stu-id="1a478-132">Response</span></span>

<span data-ttu-id="1a478-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a478-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
