---
title: 删除 userSource
description: 删除一个 userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 150bf4eb1178b30dc1d76d4276a5164412255a6d
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597588"
---
# <a name="delete-usersource"></a><span data-ttu-id="5b754-103">删除 userSource</span><span class="sxs-lookup"><span data-stu-id="5b754-103">Delete userSource</span></span>

<span data-ttu-id="5b754-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b754-105">删除 [userSource](../resources/usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b754-105">Delete a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b754-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b754-106">Permissions</span></span>

<span data-ttu-id="5b754-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b754-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b754-109">Permission type</span></span>|<span data-ttu-id="5b754-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b754-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b754-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b754-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b754-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="5b754-112">User.Read</span></span>|
|<span data-ttu-id="5b754-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b754-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b754-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b754-114">Not supported.</span></span>|
|<span data-ttu-id="5b754-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b754-115">Application</span></span>|<span data-ttu-id="5b754-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b754-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b754-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b754-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="5b754-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b754-118">Request headers</span></span>

|<span data-ttu-id="5b754-119">名称</span><span class="sxs-lookup"><span data-stu-id="5b754-119">Name</span></span>|<span data-ttu-id="5b754-120">说明</span><span class="sxs-lookup"><span data-stu-id="5b754-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b754-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b754-121">Authorization</span></span>|<span data-ttu-id="5b754-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b754-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b754-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b754-124">Request body</span></span>

<span data-ttu-id="5b754-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b754-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b754-126">响应</span><span class="sxs-lookup"><span data-stu-id="5b754-126">Response</span></span>

<span data-ttu-id="5b754-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5b754-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5b754-128">示例</span><span class="sxs-lookup"><span data-stu-id="5b754-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b754-129">请求</span><span class="sxs-lookup"><span data-stu-id="5b754-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```

### <a name="response"></a><span data-ttu-id="5b754-130">响应</span><span class="sxs-lookup"><span data-stu-id="5b754-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
