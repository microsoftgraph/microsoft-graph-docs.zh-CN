---
title: 删除 itemPhone
description: 从用户的配置文件中删除 itemPhone 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f66130b9c898865926acf728e0dfc79447530d83
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999349"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="26dff-103">删除 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="26dff-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="26dff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26dff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26dff-105">从用户的[配置文件](../resources/profile.md)中删除[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26dff-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26dff-106">权限</span><span class="sxs-lookup"><span data-stu-id="26dff-106">Permissions</span></span>

<span data-ttu-id="26dff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26dff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26dff-109">Permission type</span></span>                        | <span data-ttu-id="26dff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26dff-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26dff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26dff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26dff-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="26dff-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="26dff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26dff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26dff-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="26dff-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="26dff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="26dff-115">Application</span></span>                            | <span data-ttu-id="26dff-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26dff-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="26dff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26dff-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /user/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="26dff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26dff-118">Request headers</span></span>

|<span data-ttu-id="26dff-119">名称</span><span class="sxs-lookup"><span data-stu-id="26dff-119">Name</span></span>|<span data-ttu-id="26dff-120">说明</span><span class="sxs-lookup"><span data-stu-id="26dff-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26dff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26dff-121">Authorization</span></span>|<span data-ttu-id="26dff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26dff-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26dff-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="26dff-124">Request body</span></span>

<span data-ttu-id="26dff-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26dff-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26dff-126">响应</span><span class="sxs-lookup"><span data-stu-id="26dff-126">Response</span></span>

<span data-ttu-id="26dff-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="26dff-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26dff-128">示例</span><span class="sxs-lookup"><span data-stu-id="26dff-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26dff-129">请求</span><span class="sxs-lookup"><span data-stu-id="26dff-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/phones/{itemPhoneId}
```

### <a name="response"></a><span data-ttu-id="26dff-130">响应</span><span class="sxs-lookup"><span data-stu-id="26dff-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


