---
title: 删除 personResponsibility
description: 删除一个 personResponsibility 对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8e5ae2fecc8c1845712b1d15161694da9c215ae1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986236"
---
# <a name="delete-personresponsibility"></a><span data-ttu-id="146b2-103">删除 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="146b2-103">Delete personResponsibility</span></span>
<span data-ttu-id="146b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="146b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="146b2-105">从用户的[配置文件](../resources/profile.md)中删除[personResponsibility](../resources/personresponsibility.md)对象。</span><span class="sxs-lookup"><span data-stu-id="146b2-105">Deletes a [personResponsibility](../resources/personresponsibility.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="146b2-106">权限</span><span class="sxs-lookup"><span data-stu-id="146b2-106">Permissions</span></span>

<span data-ttu-id="146b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="146b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="146b2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="146b2-109">Permission type</span></span>                        | <span data-ttu-id="146b2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="146b2-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="146b2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="146b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="146b2-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="146b2-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="146b2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="146b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="146b2-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="146b2-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="146b2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="146b2-115">Application</span></span>                            | <span data-ttu-id="146b2-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="146b2-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="146b2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="146b2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="146b2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="146b2-118">Request headers</span></span>
|<span data-ttu-id="146b2-119">名称</span><span class="sxs-lookup"><span data-stu-id="146b2-119">Name</span></span>|<span data-ttu-id="146b2-120">说明</span><span class="sxs-lookup"><span data-stu-id="146b2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="146b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="146b2-121">Authorization</span></span>|<span data-ttu-id="146b2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="146b2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="146b2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="146b2-124">Request body</span></span>
<span data-ttu-id="146b2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="146b2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="146b2-126">响应</span><span class="sxs-lookup"><span data-stu-id="146b2-126">Response</span></span>

<span data-ttu-id="146b2-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="146b2-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="146b2-128">示例</span><span class="sxs-lookup"><span data-stu-id="146b2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="146b2-129">请求</span><span class="sxs-lookup"><span data-stu-id="146b2-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="146b2-130">响应</span><span class="sxs-lookup"><span data-stu-id="146b2-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


