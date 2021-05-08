---
title: 获取 authenticationFlowsPolicy
description: 读取 authenticationFlowsPolicy 对象的属性和关系。
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ea7ff58290c8924144b3cbd30800f2886cd56039
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231946"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="5aec0-103">获取 authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="5aec0-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="5aec0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aec0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aec0-105">读取 [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5aec0-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aec0-106">权限</span><span class="sxs-lookup"><span data-stu-id="5aec0-106">Permissions</span></span>
<span data-ttu-id="5aec0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5aec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aec0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5aec0-109">Permission type</span></span>|<span data-ttu-id="5aec0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5aec0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5aec0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5aec0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5aec0-112">Policy.Read.All、Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="5aec0-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="5aec0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5aec0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5aec0-114">不支持</span><span class="sxs-lookup"><span data-stu-id="5aec0-114">Not Supported</span></span>|
|<span data-ttu-id="5aec0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5aec0-115">Application</span></span>|<span data-ttu-id="5aec0-116">Policy.Read.All、Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="5aec0-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="5aec0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5aec0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="5aec0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5aec0-118">Request headers</span></span>
|<span data-ttu-id="5aec0-119">名称</span><span class="sxs-lookup"><span data-stu-id="5aec0-119">Name</span></span>|<span data-ttu-id="5aec0-120">说明</span><span class="sxs-lookup"><span data-stu-id="5aec0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5aec0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aec0-121">Authorization</span></span>|<span data-ttu-id="5aec0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5aec0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aec0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5aec0-124">Request body</span></span>
<span data-ttu-id="5aec0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5aec0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aec0-126">响应</span><span class="sxs-lookup"><span data-stu-id="5aec0-126">Response</span></span>

<span data-ttu-id="5aec0-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5aec0-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5aec0-128">示例</span><span class="sxs-lookup"><span data-stu-id="5aec0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5aec0-129">请求</span><span class="sxs-lookup"><span data-stu-id="5aec0-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5aec0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aec0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```
# <a name="c"></a>[<span data-ttu-id="5aec0-131">C#</span><span class="sxs-lookup"><span data-stu-id="5aec0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aec0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aec0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aec0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aec0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aec0-134">Java</span><span class="sxs-lookup"><span data-stu-id="5aec0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationflowspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5aec0-135">响应</span><span class="sxs-lookup"><span data-stu-id="5aec0-135">Response</span></span>
<span data-ttu-id="5aec0-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5aec0-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy"
}
-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationFlowsPolicy/$entity",
    "id": "authenticationFlowsPolicy",
    "displayName": "Authentication flows policy",
    "description": "Authentication flows policy allows modification of settings related to authentication flows in AAD tenant, such as self-service sign up configuration.",
    "selfServiceSignUp": {
        "isEnabled": true
    }
}
```


