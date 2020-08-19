---
title: 删除 personResponsibility
description: 删除一个 personResponsibility 对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bb99620a23370f6763fa6544a3992053f5057183
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812937"
---
# <a name="delete-personresponsibility"></a><span data-ttu-id="97724-103">删除 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="97724-103">Delete personResponsibility</span></span>
<span data-ttu-id="97724-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97724-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97724-105">从用户的[配置文件](../resources/profile.md)中删除[personResponsibility](../resources/personresponsibility.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97724-105">Deletes a [personResponsibility](../resources/personresponsibility.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97724-106">权限</span><span class="sxs-lookup"><span data-stu-id="97724-106">Permissions</span></span>

<span data-ttu-id="97724-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97724-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97724-109">Permission type</span></span>                        | <span data-ttu-id="97724-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97724-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="97724-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97724-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="97724-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="97724-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="97724-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97724-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97724-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="97724-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="97724-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97724-115">Application</span></span>                            | <span data-ttu-id="97724-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="97724-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="97724-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97724-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97724-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="97724-118">Request headers</span></span>
|<span data-ttu-id="97724-119">名称</span><span class="sxs-lookup"><span data-stu-id="97724-119">Name</span></span>|<span data-ttu-id="97724-120">说明</span><span class="sxs-lookup"><span data-stu-id="97724-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97724-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97724-121">Authorization</span></span>|<span data-ttu-id="97724-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97724-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97724-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="97724-124">Request body</span></span>
<span data-ttu-id="97724-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97724-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97724-126">响应</span><span class="sxs-lookup"><span data-stu-id="97724-126">Response</span></span>

<span data-ttu-id="97724-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="97724-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="97724-128">示例</span><span class="sxs-lookup"><span data-stu-id="97724-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97724-129">请求</span><span class="sxs-lookup"><span data-stu-id="97724-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="97724-130">响应</span><span class="sxs-lookup"><span data-stu-id="97724-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
