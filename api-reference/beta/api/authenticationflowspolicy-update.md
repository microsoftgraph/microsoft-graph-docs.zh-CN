---
title: 更新 authenticationFlowsPolicy
description: 更新 authenticationFlowsPolicy 对象的布尔 selfServiceSignUp 属性。
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3408cff98cc79dbf819e077ab12fa066f7d723f7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680881"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="f9bcd-103">更新 authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="f9bcd-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="f9bcd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9bcd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9bcd-105">更新[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)对象的布尔**selfServiceSignUp**属性。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-105">Update the Boolean **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="f9bcd-106">无法修改属性**id**、**类型**和**说明**。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9bcd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9bcd-107">Permissions</span></span>
<span data-ttu-id="f9bcd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9bcd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9bcd-110">Permission type</span></span>|<span data-ttu-id="f9bcd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9bcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9bcd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9bcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9bcd-113">AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="f9bcd-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="f9bcd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9bcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9bcd-115">不支持</span><span class="sxs-lookup"><span data-stu-id="f9bcd-115">Not Supported</span></span>|
|<span data-ttu-id="f9bcd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9bcd-116">Application</span></span>|<span data-ttu-id="f9bcd-117">AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="f9bcd-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9bcd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9bcd-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="f9bcd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9bcd-119">Request headers</span></span>
|<span data-ttu-id="f9bcd-120">名称</span><span class="sxs-lookup"><span data-stu-id="f9bcd-120">Name</span></span>|<span data-ttu-id="f9bcd-121">说明</span><span class="sxs-lookup"><span data-stu-id="f9bcd-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9bcd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9bcd-122">Authorization</span></span>|<span data-ttu-id="f9bcd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f9bcd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9bcd-125">Content-Type</span></span>|<span data-ttu-id="f9bcd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f9bcd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9bcd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9bcd-128">Request body</span></span>
<span data-ttu-id="f9bcd-129">在请求正文中，可以提供[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)对象的 JSON 表示形式（但不是必需的）。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object (but is not required.)</span></span>

<span data-ttu-id="f9bcd-130">下表显示了在更新[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="f9bcd-131">属性</span><span class="sxs-lookup"><span data-stu-id="f9bcd-131">Property</span></span>|<span data-ttu-id="f9bcd-132">类型</span><span class="sxs-lookup"><span data-stu-id="f9bcd-132">Type</span></span>|<span data-ttu-id="f9bcd-133">Description</span><span class="sxs-lookup"><span data-stu-id="f9bcd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9bcd-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="f9bcd-134">selfServiceSignUp</span></span>|[<span data-ttu-id="f9bcd-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9bcd-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="f9bcd-136">自助注册配置。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="f9bcd-137">响应</span><span class="sxs-lookup"><span data-stu-id="f9bcd-137">Response</span></span>

<span data-ttu-id="f9bcd-138">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="f9bcd-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9bcd-139">示例</span><span class="sxs-lookup"><span data-stu-id="f9bcd-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9bcd-140">请求</span><span class="sxs-lookup"><span data-stu-id="f9bcd-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f9bcd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9bcd-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f9bcd-142">C#</span><span class="sxs-lookup"><span data-stu-id="f9bcd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9bcd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9bcd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9bcd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9bcd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9bcd-145">响应</span><span class="sxs-lookup"><span data-stu-id="f9bcd-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
