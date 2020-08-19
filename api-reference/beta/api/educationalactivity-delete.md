---
title: 删除 educationalActivity
description: 从用户配置文件中删除 educationalActivity 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 96c717171f683d2a32e62b4e79b80639e2cb5242
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810949"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="744e9-103">删除 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="744e9-103">Delete educationalActivity</span></span>

<span data-ttu-id="744e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="744e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="744e9-105">从用户的[配置文件](../resources/profile.md)中删除[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="744e9-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="744e9-106">权限</span><span class="sxs-lookup"><span data-stu-id="744e9-106">Permissions</span></span>

<span data-ttu-id="744e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="744e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="744e9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="744e9-109">Permission type</span></span>                        | <span data-ttu-id="744e9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="744e9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="744e9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="744e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="744e9-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="744e9-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="744e9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="744e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="744e9-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="744e9-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="744e9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="744e9-115">Application</span></span>                            | <span data-ttu-id="744e9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="744e9-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="744e9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="744e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
DELETE /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="744e9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="744e9-118">Request headers</span></span>

| <span data-ttu-id="744e9-119">名称</span><span class="sxs-lookup"><span data-stu-id="744e9-119">Name</span></span>           |<span data-ttu-id="744e9-120">说明</span><span class="sxs-lookup"><span data-stu-id="744e9-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="744e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="744e9-121">Authorization</span></span>  | <span data-ttu-id="744e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="744e9-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="744e9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="744e9-124">Request body</span></span>

<span data-ttu-id="744e9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="744e9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="744e9-126">响应</span><span class="sxs-lookup"><span data-stu-id="744e9-126">Response</span></span>

<span data-ttu-id="744e9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="744e9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="744e9-129">示例</span><span class="sxs-lookup"><span data-stu-id="744e9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="744e9-130">请求</span><span class="sxs-lookup"><span data-stu-id="744e9-130">Request</span></span>

<span data-ttu-id="744e9-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="744e9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```

### <a name="response"></a><span data-ttu-id="744e9-132">响应</span><span class="sxs-lookup"><span data-stu-id="744e9-132">Response</span></span>

<span data-ttu-id="744e9-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="744e9-133">The following is an example of the response.</span></span>

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
