---
title: 获取 authenticationListener
description: 读取 authenticationListener 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e6cacb31a31963457c2e37fd9a63d1c0eeea2c6c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438482"
---
# <a name="get-authenticationlistener"></a><span data-ttu-id="b8f54-103">获取 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="b8f54-103">Get authenticationListener</span></span>

<span data-ttu-id="b8f54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8f54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8f54-105">获取为身份验证管道中的 onSignupStart 事件定义的指定[authenticationListener。](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="b8f54-105">Get the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8f54-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b8f54-106">Permissions</span></span>

<span data-ttu-id="b8f54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8f54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8f54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8f54-109">Permission type</span></span>|<span data-ttu-id="b8f54-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8f54-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8f54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8f54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8f54-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8f54-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="b8f54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8f54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8f54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8f54-114">Not supported.</span></span>|
|<span data-ttu-id="b8f54-115">Application</span><span class="sxs-lookup"><span data-stu-id="b8f54-115">Application</span></span>|<span data-ttu-id="b8f54-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8f54-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8f54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8f54-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8f54-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b8f54-118">Optional query parameters</span></span>

<span data-ttu-id="b8f54-119">此方法支持 `$expand` OData 查询参数扩展 invokeUserFlowListener 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b8f54-119">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="b8f54-120">有关示例，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="b8f54-120">See below for an example.</span></span> <span data-ttu-id="b8f54-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b8f54-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8f54-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8f54-122">Request headers</span></span>

|<span data-ttu-id="b8f54-123">名称</span><span class="sxs-lookup"><span data-stu-id="b8f54-123">Name</span></span>|<span data-ttu-id="b8f54-124">说明</span><span class="sxs-lookup"><span data-stu-id="b8f54-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b8f54-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8f54-125">Authorization</span></span>|<span data-ttu-id="b8f54-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8f54-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8f54-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8f54-128">Request body</span></span>

<span data-ttu-id="b8f54-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8f54-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8f54-130">响应</span><span class="sxs-lookup"><span data-stu-id="b8f54-130">Response</span></span>

<span data-ttu-id="b8f54-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [authenticationListener](../resources/authenticationlistener.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8f54-131">If successful, this method returns a `200 OK` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8f54-132">示例</span><span class="sxs-lookup"><span data-stu-id="b8f54-132">Examples</span></span>

### <a name="example-1-get-an-authenticationlistener-by-id"></a><span data-ttu-id="b8f54-133">示例 1：按 id 获取 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="b8f54-133">Example 1: Get an authenticationListener by id</span></span>

#### <a name="request"></a><span data-ttu-id="b8f54-134">请求</span><span class="sxs-lookup"><span data-stu-id="b8f54-134">Request</span></span>

<span data-ttu-id="b8f54-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b8f54-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a><span data-ttu-id="b8f54-136">响应</span><span class="sxs-lookup"><span data-stu-id="b8f54-136">Response</span></span>

<span data-ttu-id="b8f54-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b8f54-137">The following is an example of the response.</span></span>

<span data-ttu-id="b8f54-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8f54-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
   }
}
```

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a><span data-ttu-id="b8f54-139">示例 2：展开特定 authenticationListener 的 invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="b8f54-139">Example 2: Expand invokeUserFlowListener for a specific authenticationListener</span></span>

<span data-ttu-id="b8f54-140">以下示例按 onSignupStart 事件的 ID 获取侦听器，并展开调用的用户流。</span><span class="sxs-lookup"><span data-stu-id="b8f54-140">The following example gets the listener by id for the onSignupStart event and expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="b8f54-141">请求</span><span class="sxs-lookup"><span data-stu-id="b8f54-141">Request</span></span>

<span data-ttu-id="b8f54-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b8f54-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a><span data-ttu-id="b8f54-143">响应</span><span class="sxs-lookup"><span data-stu-id="b8f54-143">Response</span></span>

<span data-ttu-id="b8f54-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b8f54-144">The following is an example of the response.</span></span>

<span data-ttu-id="b8f54-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8f54-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invokeUserFlowListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
  },
  "userFlow": {
      "id": "B2X_1_Partner",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationListener",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
