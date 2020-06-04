---
title: 更新 authenticationFlowsPolicy
description: 更新 authenticationFlowsPolicy 对象的布尔 selfServiceSignUp 属性。
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 626e1dc8a851f2c8da6a9bb815a4e783cf44e7d2
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556384"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="257e4-103">更新 authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="257e4-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="257e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="257e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="257e4-105">更新[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)对象的布尔**selfServiceSignUp**属性。</span><span class="sxs-lookup"><span data-stu-id="257e4-105">Update the Boolean **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="257e4-106">无法修改属性**id**、**类型**和**说明**。</span><span class="sxs-lookup"><span data-stu-id="257e4-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="257e4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="257e4-107">Permissions</span></span>
<span data-ttu-id="257e4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="257e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="257e4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="257e4-110">Permission type</span></span>|<span data-ttu-id="257e4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="257e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="257e4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="257e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="257e4-113">AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="257e4-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="257e4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="257e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="257e4-115">不支持</span><span class="sxs-lookup"><span data-stu-id="257e4-115">Not Supported</span></span>|
|<span data-ttu-id="257e4-116">Application</span><span class="sxs-lookup"><span data-stu-id="257e4-116">Application</span></span>|<span data-ttu-id="257e4-117">AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="257e4-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="257e4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="257e4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="257e4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="257e4-119">Request headers</span></span>
|<span data-ttu-id="257e4-120">名称</span><span class="sxs-lookup"><span data-stu-id="257e4-120">Name</span></span>|<span data-ttu-id="257e4-121">说明</span><span class="sxs-lookup"><span data-stu-id="257e4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="257e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="257e4-122">Authorization</span></span>|<span data-ttu-id="257e4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="257e4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="257e4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="257e4-125">Content-Type</span></span>|<span data-ttu-id="257e4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="257e4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="257e4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="257e4-128">Request body</span></span>
<span data-ttu-id="257e4-129">在请求正文中，可以提供[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)对象的 JSON 表示形式（但不是必需的）。</span><span class="sxs-lookup"><span data-stu-id="257e4-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object (but is not required.)</span></span>

<span data-ttu-id="257e4-130">下表显示了在更新[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="257e4-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="257e4-131">属性</span><span class="sxs-lookup"><span data-stu-id="257e4-131">Property</span></span>|<span data-ttu-id="257e4-132">类型</span><span class="sxs-lookup"><span data-stu-id="257e4-132">Type</span></span>|<span data-ttu-id="257e4-133">说明</span><span class="sxs-lookup"><span data-stu-id="257e4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="257e4-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="257e4-134">selfServiceSignUp</span></span>|[<span data-ttu-id="257e4-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="257e4-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="257e4-136">自助注册配置。</span><span class="sxs-lookup"><span data-stu-id="257e4-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="257e4-137">响应</span><span class="sxs-lookup"><span data-stu-id="257e4-137">Response</span></span>

<span data-ttu-id="257e4-138">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="257e4-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="257e4-139">示例</span><span class="sxs-lookup"><span data-stu-id="257e4-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="257e4-140">请求</span><span class="sxs-lookup"><span data-stu-id="257e4-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->
```http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### <a name="response"></a><span data-ttu-id="257e4-141">响应</span><span class="sxs-lookup"><span data-stu-id="257e4-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
