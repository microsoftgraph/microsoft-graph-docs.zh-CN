---
title: 更新 authenticationListener
description: 更新为身份验证管道中的事件定义的侦听器。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5acb660843bf0b7a60fd66886841ab4c490f396
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872392"
---
# <a name="update-authenticationlistener"></a><span data-ttu-id="7c771-103">更新 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="7c771-103">Update authenticationListener</span></span>

<span data-ttu-id="7c771-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c771-105">更新为身份验证管道中的事件定义的[authenticationListener。](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="7c771-105">Update the [authenticationListener](../resources/authenticationlistener.md) defined for an event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c771-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c771-106">Permissions</span></span>

<span data-ttu-id="7c771-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c771-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c771-109">Permission type</span></span>|<span data-ttu-id="7c771-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c771-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c771-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c771-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c771-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c771-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="7c771-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c771-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c771-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c771-114">Not supported.</span></span>|
|<span data-ttu-id="7c771-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c771-115">Application</span></span>|<span data-ttu-id="7c771-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c771-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c771-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c771-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7c771-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c771-118">Request headers</span></span>

|<span data-ttu-id="7c771-119">名称</span><span class="sxs-lookup"><span data-stu-id="7c771-119">Name</span></span>|<span data-ttu-id="7c771-120">说明</span><span class="sxs-lookup"><span data-stu-id="7c771-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7c771-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c771-121">Authorization</span></span>|<span data-ttu-id="7c771-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c771-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c771-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c771-124">Content-Type</span></span>|<span data-ttu-id="7c771-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7c771-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c771-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c771-127">Request body</span></span>

<span data-ttu-id="7c771-128">在请求正文中，提供 [authenticationListener](../resources/authenticationlistener.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c771-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="7c771-129">下表显示更新 [invokeUserFlowAction](../resources/invokeuserflowlistener.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7c771-129">The following table shows the properties that are required when you update the [invokeUserFlowAction](../resources/invokeuserflowlistener.md).</span></span>

|<span data-ttu-id="7c771-130">属性</span><span class="sxs-lookup"><span data-stu-id="7c771-130">Property</span></span>|<span data-ttu-id="7c771-131">类型</span><span class="sxs-lookup"><span data-stu-id="7c771-131">Type</span></span>|<span data-ttu-id="7c771-132">Description</span><span class="sxs-lookup"><span data-stu-id="7c771-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c771-133">priority</span><span class="sxs-lookup"><span data-stu-id="7c771-133">priority</span></span>|<span data-ttu-id="7c771-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7c771-134">Int32</span></span>|<span data-ttu-id="7c771-135">侦听器的优先级。</span><span class="sxs-lookup"><span data-stu-id="7c771-135">The priority of the listener.</span></span> <span data-ttu-id="7c771-136">确定事件具有多个侦听器时的评估顺序。</span><span class="sxs-lookup"><span data-stu-id="7c771-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="7c771-137">优先级从低到高进行评估。</span><span class="sxs-lookup"><span data-stu-id="7c771-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="7c771-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="7c771-138">sourceFilter</span></span>|[<span data-ttu-id="7c771-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="7c771-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="7c771-140">基于用于确定是否评估侦听器的身份验证源进行筛选。</span><span class="sxs-lookup"><span data-stu-id="7c771-140">Filter based on the source of the authentication which is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="7c771-141">当前仅限于基于用户进行身份验证的应用程序的评估。</span><span class="sxs-lookup"><span data-stu-id="7c771-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="response"></a><span data-ttu-id="7c771-142">响应</span><span class="sxs-lookup"><span data-stu-id="7c771-142">Response</span></span>

<span data-ttu-id="7c771-143">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7c771-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7c771-144">示例</span><span class="sxs-lookup"><span data-stu-id="7c771-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c771-145">请求</span><span class="sxs-lookup"><span data-stu-id="7c771-145">Request</span></span>

<span data-ttu-id="7c771-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c771-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_onsignupstart"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
  "priority": 101
}
```

### <a name="response"></a><span data-ttu-id="7c771-147">响应</span><span class="sxs-lookup"><span data-stu-id="7c771-147">Response</span></span>

<span data-ttu-id="7c771-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c771-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
