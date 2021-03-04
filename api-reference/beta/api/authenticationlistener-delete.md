---
title: 删除 authenticationListener
description: 从 authenticationEventsPolicy 支持的事件中删除 authenticationListener。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c808aa161bacb2612c90a53f58b7163f663e4150
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438489"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="8a359-103">删除 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="8a359-103">Remove authenticationListener</span></span>

<span data-ttu-id="8a359-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a359-105">删除为身份验证管道中的 onSignupStart 事件定义的指定[authenticationListener。](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="8a359-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a359-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8a359-106">Permissions</span></span>

<span data-ttu-id="8a359-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a359-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a359-109">Permission type</span></span>|<span data-ttu-id="8a359-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a359-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a359-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a359-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a359-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a359-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="8a359-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a359-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a359-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a359-114">Not supported.</span></span>|
|<span data-ttu-id="8a359-115">Application</span><span class="sxs-lookup"><span data-stu-id="8a359-115">Application</span></span>|<span data-ttu-id="8a359-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a359-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a359-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a359-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a359-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a359-118">Request headers</span></span>

|<span data-ttu-id="8a359-119">名称</span><span class="sxs-lookup"><span data-stu-id="8a359-119">Name</span></span>|<span data-ttu-id="8a359-120">说明</span><span class="sxs-lookup"><span data-stu-id="8a359-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a359-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a359-121">Authorization</span></span>|<span data-ttu-id="8a359-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a359-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a359-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a359-124">Request body</span></span>

<span data-ttu-id="8a359-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a359-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a359-126">响应</span><span class="sxs-lookup"><span data-stu-id="8a359-126">Response</span></span>

<span data-ttu-id="8a359-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8a359-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8a359-128">示例</span><span class="sxs-lookup"><span data-stu-id="8a359-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a359-129">请求</span><span class="sxs-lookup"><span data-stu-id="8a359-129">Request</span></span>

<span data-ttu-id="8a359-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a359-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="8a359-131">响应</span><span class="sxs-lookup"><span data-stu-id="8a359-131">Response</span></span>

<span data-ttu-id="8a359-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8a359-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
