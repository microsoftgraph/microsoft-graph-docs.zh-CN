---
title: 删除 personResponsibility
description: 删除 personResponsibility 对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 17ce90f05b52cb05c3030ceff0fb3312f71466ef
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292719"
---
# <a name="delete-personresponsibility"></a><span data-ttu-id="f6e41-103">删除 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="f6e41-103">Delete personResponsibility</span></span>
<span data-ttu-id="f6e41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6e41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6e41-105">从用户配置文件 [中删除 personResponsibility](../resources/personresponsibility.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="f6e41-105">Deletes a [personResponsibility](../resources/personresponsibility.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6e41-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6e41-106">Permissions</span></span>

<span data-ttu-id="f6e41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6e41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6e41-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6e41-109">Permission type</span></span>                        | <span data-ttu-id="f6e41-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6e41-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f6e41-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6e41-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6e41-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e41-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f6e41-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6e41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6e41-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e41-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f6e41-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6e41-115">Application</span></span>                            | <span data-ttu-id="f6e41-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6e41-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f6e41-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6e41-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6e41-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6e41-118">Request headers</span></span>
|<span data-ttu-id="f6e41-119">名称</span><span class="sxs-lookup"><span data-stu-id="f6e41-119">Name</span></span>|<span data-ttu-id="f6e41-120">说明</span><span class="sxs-lookup"><span data-stu-id="f6e41-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6e41-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6e41-121">Authorization</span></span>|<span data-ttu-id="f6e41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6e41-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6e41-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6e41-124">Request body</span></span>
<span data-ttu-id="f6e41-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6e41-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6e41-126">响应</span><span class="sxs-lookup"><span data-stu-id="f6e41-126">Response</span></span>

<span data-ttu-id="f6e41-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f6e41-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f6e41-128">示例</span><span class="sxs-lookup"><span data-stu-id="f6e41-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6e41-129">请求</span><span class="sxs-lookup"><span data-stu-id="f6e41-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="f6e41-130">响应</span><span class="sxs-lookup"><span data-stu-id="f6e41-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


