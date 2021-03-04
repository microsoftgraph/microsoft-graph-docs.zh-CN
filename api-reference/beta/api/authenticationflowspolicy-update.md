---
title: 更新 authenticationFlowsPolicy
description: 更新 authenticationFlowsPolicy 对象的布尔 Boolean selfServiceSignUp 属性。
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3e0ad7345b7017ec543bb4813b62edb71fb77f21
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438510"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="05146-103">更新 authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="05146-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="05146-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05146-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05146-105">更新 [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) 对象的布尔 **selfServiceSignUp** 属性。</span><span class="sxs-lookup"><span data-stu-id="05146-105">Update the Boolean **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="05146-106">无法修改 **id**、**type** 和 **description** 属性。</span><span class="sxs-lookup"><span data-stu-id="05146-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="05146-107">权限</span><span class="sxs-lookup"><span data-stu-id="05146-107">Permissions</span></span>
<span data-ttu-id="05146-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05146-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05146-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="05146-110">Permission type</span></span>|<span data-ttu-id="05146-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05146-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05146-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05146-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05146-113">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="05146-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="05146-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05146-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05146-115">不支持</span><span class="sxs-lookup"><span data-stu-id="05146-115">Not Supported</span></span>|
|<span data-ttu-id="05146-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="05146-116">Application</span></span>|<span data-ttu-id="05146-117">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="05146-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="05146-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05146-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="05146-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="05146-119">Request headers</span></span>
|<span data-ttu-id="05146-120">名称</span><span class="sxs-lookup"><span data-stu-id="05146-120">Name</span></span>|<span data-ttu-id="05146-121">说明</span><span class="sxs-lookup"><span data-stu-id="05146-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05146-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05146-122">Authorization</span></span>|<span data-ttu-id="05146-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05146-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05146-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05146-125">Content-Type</span></span>|<span data-ttu-id="05146-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="05146-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05146-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="05146-128">Request body</span></span>
<span data-ttu-id="05146-129">在请求正文中，你可以提供 [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) 对象的 JSON 表示形式（但不是必需的）。</span><span class="sxs-lookup"><span data-stu-id="05146-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object (but is not required.)</span></span>

<span data-ttu-id="05146-130">下表显示了更新 [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05146-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="05146-131">属性</span><span class="sxs-lookup"><span data-stu-id="05146-131">Property</span></span>|<span data-ttu-id="05146-132">类型</span><span class="sxs-lookup"><span data-stu-id="05146-132">Type</span></span>|<span data-ttu-id="05146-133">说明</span><span class="sxs-lookup"><span data-stu-id="05146-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05146-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="05146-134">selfServiceSignUp</span></span>|[<span data-ttu-id="05146-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="05146-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="05146-136">自助注册配置。</span><span class="sxs-lookup"><span data-stu-id="05146-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="05146-137">响应</span><span class="sxs-lookup"><span data-stu-id="05146-137">Response</span></span>

<span data-ttu-id="05146-138">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="05146-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="05146-139">示例</span><span class="sxs-lookup"><span data-stu-id="05146-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="05146-140">请求</span><span class="sxs-lookup"><span data-stu-id="05146-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="05146-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="05146-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="05146-142">C#</span><span class="sxs-lookup"><span data-stu-id="05146-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05146-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05146-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05146-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05146-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05146-145">Java</span><span class="sxs-lookup"><span data-stu-id="05146-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationflowspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05146-146">响应</span><span class="sxs-lookup"><span data-stu-id="05146-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```


