---
title: 获取 authenticationListener
description: 读取 authenticationListener 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3e6f07ac59e143ab7e9723c5a5b81a4c8489e54
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872420"
---
# <a name="get-authenticationlistener"></a><span data-ttu-id="7593f-103">获取 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="7593f-103">Get authenticationListener</span></span>

<span data-ttu-id="7593f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7593f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7593f-105">获取为身份验证管道中的 onSignupStart 事件定义的指定[authenticationListener。](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="7593f-105">Get the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="7593f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7593f-106">Permissions</span></span>

<span data-ttu-id="7593f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7593f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7593f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7593f-109">Permission type</span></span>|<span data-ttu-id="7593f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7593f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7593f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7593f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7593f-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7593f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="7593f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7593f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7593f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7593f-114">Not supported.</span></span>|
|<span data-ttu-id="7593f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7593f-115">Application</span></span>|<span data-ttu-id="7593f-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7593f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="7593f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7593f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7593f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7593f-118">Optional query parameters</span></span>

<span data-ttu-id="7593f-119">此方法支持 `$expand` OData 查询参数扩展 invokeUserFlowListener 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7593f-119">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="7593f-120">有关示例，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="7593f-120">See below for an example.</span></span> <span data-ttu-id="7593f-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7593f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7593f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7593f-122">Request headers</span></span>

|<span data-ttu-id="7593f-123">名称</span><span class="sxs-lookup"><span data-stu-id="7593f-123">Name</span></span>|<span data-ttu-id="7593f-124">说明</span><span class="sxs-lookup"><span data-stu-id="7593f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7593f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7593f-125">Authorization</span></span>|<span data-ttu-id="7593f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7593f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7593f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7593f-128">Request body</span></span>

<span data-ttu-id="7593f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7593f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7593f-130">响应</span><span class="sxs-lookup"><span data-stu-id="7593f-130">Response</span></span>

<span data-ttu-id="7593f-131">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [authenticationListener](../resources/authenticationlistener.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7593f-131">If successful, this method returns a `200 OK` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7593f-132">示例</span><span class="sxs-lookup"><span data-stu-id="7593f-132">Examples</span></span>

### <a name="example-1-get-an-authenticationlistener-by-id"></a><span data-ttu-id="7593f-133">示例 1：按 ID 获取 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="7593f-133">Example 1: Get an authenticationListener by id</span></span>

#### <a name="request"></a><span data-ttu-id="7593f-134">请求</span><span class="sxs-lookup"><span data-stu-id="7593f-134">Request</span></span>

<span data-ttu-id="7593f-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7593f-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a><span data-ttu-id="7593f-136">响应</span><span class="sxs-lookup"><span data-stu-id="7593f-136">Response</span></span>

<span data-ttu-id="7593f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7593f-137">The following is an example of the response.</span></span>

<span data-ttu-id="7593f-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7593f-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a><span data-ttu-id="7593f-139">示例 2：展开特定 authenticationListener 的 invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="7593f-139">Example 2: Expand invokeUserFlowListener for a specific authenticationListener</span></span>

<span data-ttu-id="7593f-140">以下示例按 id 获取 onSignupStart 事件的侦听器，并展开调用的用户流。</span><span class="sxs-lookup"><span data-stu-id="7593f-140">The following example gets the listener by id for the onSignupStart event and expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="7593f-141">请求</span><span class="sxs-lookup"><span data-stu-id="7593f-141">Request</span></span>

<span data-ttu-id="7593f-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7593f-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a><span data-ttu-id="7593f-143">响应</span><span class="sxs-lookup"><span data-stu-id="7593f-143">Response</span></span>

<span data-ttu-id="7593f-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7593f-144">The following is an example of the response.</span></span>

<span data-ttu-id="7593f-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7593f-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
