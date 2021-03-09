---
title: 删除 itemPhone
description: 从用户配置文件中删除 itemPhone 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4b947a7674f73a4351cdb6742587812acd66d253
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577413"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="ed873-103">删除 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ed873-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="ed873-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed873-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed873-105">从用户配置文件中删除 [itemPhone](../resources/itemphone.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="ed873-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed873-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed873-106">Permissions</span></span>

<span data-ttu-id="ed873-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed873-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed873-109">Permission type</span></span>                        | <span data-ttu-id="ed873-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed873-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed873-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed873-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed873-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed873-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ed873-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed873-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed873-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed873-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ed873-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed873-115">Application</span></span>                            | <span data-ttu-id="ed873-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed873-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ed873-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed873-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /users/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="ed873-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed873-118">Request headers</span></span>

|<span data-ttu-id="ed873-119">名称</span><span class="sxs-lookup"><span data-stu-id="ed873-119">Name</span></span>|<span data-ttu-id="ed873-120">说明</span><span class="sxs-lookup"><span data-stu-id="ed873-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed873-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed873-121">Authorization</span></span>|<span data-ttu-id="ed873-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed873-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed873-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed873-124">Request body</span></span>

<span data-ttu-id="ed873-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed873-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed873-126">响应</span><span class="sxs-lookup"><span data-stu-id="ed873-126">Response</span></span>

<span data-ttu-id="ed873-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ed873-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ed873-128">示例</span><span class="sxs-lookup"><span data-stu-id="ed873-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed873-129">请求</span><span class="sxs-lookup"><span data-stu-id="ed873-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/phones/{itemPhoneId}
```

### <a name="response"></a><span data-ttu-id="ed873-130">响应</span><span class="sxs-lookup"><span data-stu-id="ed873-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


