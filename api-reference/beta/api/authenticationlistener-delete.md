---
title: 删除 authenticationListener
description: 从 authenticationEventsPolicy 支持的事件中删除 authenticationListener。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3db702f80e92ce475d0b3699236096d7d7b79392
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872322"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="60f88-103">删除 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="60f88-103">Remove authenticationListener</span></span>

<span data-ttu-id="60f88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60f88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60f88-105">删除为身份验证管道中的 onSignupStart 事件定义的指定[authenticationListener。](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="60f88-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="60f88-106">权限</span><span class="sxs-lookup"><span data-stu-id="60f88-106">Permissions</span></span>

<span data-ttu-id="60f88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60f88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60f88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60f88-109">Permission type</span></span>|<span data-ttu-id="60f88-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60f88-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60f88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60f88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60f88-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="60f88-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="60f88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60f88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60f88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="60f88-114">Not supported.</span></span>|
|<span data-ttu-id="60f88-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="60f88-115">Application</span></span>|<span data-ttu-id="60f88-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="60f88-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="60f88-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60f88-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60f88-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="60f88-118">Request headers</span></span>

|<span data-ttu-id="60f88-119">名称</span><span class="sxs-lookup"><span data-stu-id="60f88-119">Name</span></span>|<span data-ttu-id="60f88-120">说明</span><span class="sxs-lookup"><span data-stu-id="60f88-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60f88-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="60f88-121">Authorization</span></span>|<span data-ttu-id="60f88-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60f88-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60f88-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="60f88-124">Request body</span></span>

<span data-ttu-id="60f88-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60f88-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60f88-126">响应</span><span class="sxs-lookup"><span data-stu-id="60f88-126">Response</span></span>

<span data-ttu-id="60f88-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="60f88-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="60f88-128">示例</span><span class="sxs-lookup"><span data-stu-id="60f88-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60f88-129">请求</span><span class="sxs-lookup"><span data-stu-id="60f88-129">Request</span></span>

<span data-ttu-id="60f88-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="60f88-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="60f88-131">响应</span><span class="sxs-lookup"><span data-stu-id="60f88-131">Response</span></span>

<span data-ttu-id="60f88-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="60f88-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
