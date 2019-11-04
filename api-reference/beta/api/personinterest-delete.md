---
title: 删除 personInterest
description: 从用户的配置文件中删除 personInterest 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ede00cecfd7ecff638a4f29ccbb42835ccd73c1c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937894"
---
# <a name="delete-personinterest"></a><span data-ttu-id="38417-103">删除 personInterest</span><span class="sxs-lookup"><span data-stu-id="38417-103">Delete personInterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38417-104">从用户的[配置文件](../resources/profile.md)中删除[personInterest](../resources/personinterest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38417-104">Delete a [personInterest](../resources/personinterest.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38417-105">权限</span><span class="sxs-lookup"><span data-stu-id="38417-105">Permissions</span></span>

<span data-ttu-id="38417-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38417-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="38417-108">Permission type</span></span>                        | <span data-ttu-id="38417-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38417-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38417-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38417-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="38417-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="38417-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38417-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38417-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38417-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="38417-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38417-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="38417-114">Application</span></span>                            | <span data-ttu-id="38417-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38417-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="38417-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38417-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38417-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="38417-117">Request headers</span></span>

| <span data-ttu-id="38417-118">名称</span><span class="sxs-lookup"><span data-stu-id="38417-118">Name</span></span>           |<span data-ttu-id="38417-119">说明</span><span class="sxs-lookup"><span data-stu-id="38417-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="38417-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38417-120">Authorization</span></span>  | <span data-ttu-id="38417-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38417-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="38417-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="38417-123">Request body</span></span>

<span data-ttu-id="38417-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38417-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38417-125">响应</span><span class="sxs-lookup"><span data-stu-id="38417-125">Response</span></span>

<span data-ttu-id="38417-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="38417-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38417-128">示例</span><span class="sxs-lookup"><span data-stu-id="38417-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38417-129">请求</span><span class="sxs-lookup"><span data-stu-id="38417-129">Request</span></span>

<span data-ttu-id="38417-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38417-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```

### <a name="response"></a><span data-ttu-id="38417-131">响应</span><span class="sxs-lookup"><span data-stu-id="38417-131">Response</span></span>

<span data-ttu-id="38417-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38417-132">The following is an example of the response.</span></span>

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
  "description": "Delete personInterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
