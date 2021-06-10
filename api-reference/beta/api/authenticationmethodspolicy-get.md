---
title: 获取 authenticationMethodsPolicy
description: 读取 authenticationMethodsPolicy 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8c4e737187726f45bb546ea16d09d3ce476401fa
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869479"
---
# <a name="get-authenticationmethodspolicy"></a><span data-ttu-id="f66aa-103">获取 authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="f66aa-103">Get authenticationMethodsPolicy</span></span>
<span data-ttu-id="f66aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f66aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f66aa-105">读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f66aa-105">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f66aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="f66aa-106">Permissions</span></span>
<span data-ttu-id="f66aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f66aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f66aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f66aa-109">Permission type</span></span>|<span data-ttu-id="f66aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f66aa-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f66aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f66aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f66aa-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f66aa-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="f66aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f66aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f66aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f66aa-114">Not supported.</span></span>|
|<span data-ttu-id="f66aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f66aa-115">Application</span></span>|<span data-ttu-id="f66aa-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f66aa-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="f66aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f66aa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f66aa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f66aa-118">Optional query parameters</span></span>
<span data-ttu-id="f66aa-119">此方法不支持任何可选的查询参数。</span><span class="sxs-lookup"><span data-stu-id="f66aa-119">This method does not support any optional query parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f66aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f66aa-120">Request headers</span></span>
|<span data-ttu-id="f66aa-121">名称</span><span class="sxs-lookup"><span data-stu-id="f66aa-121">Name</span></span>|<span data-ttu-id="f66aa-122">说明</span><span class="sxs-lookup"><span data-stu-id="f66aa-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f66aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f66aa-123">Authorization</span></span>|<span data-ttu-id="f66aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f66aa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f66aa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f66aa-126">Request body</span></span>
<span data-ttu-id="f66aa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f66aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f66aa-128">响应</span><span class="sxs-lookup"><span data-stu-id="f66aa-128">Response</span></span>

<span data-ttu-id="f66aa-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f66aa-129">If successful, this method returns a `200 OK` response code and an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f66aa-130">示例</span><span class="sxs-lookup"><span data-stu-id="f66aa-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f66aa-131">请求</span><span class="sxs-lookup"><span data-stu-id="f66aa-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f66aa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f66aa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```
# <a name="c"></a>[<span data-ttu-id="f66aa-133">C#</span><span class="sxs-lookup"><span data-stu-id="f66aa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f66aa-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f66aa-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f66aa-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f66aa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f66aa-136">Java</span><span class="sxs-lookup"><span data-stu-id="f66aa-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f66aa-137">响应</span><span class="sxs-lookup"><span data-stu-id="f66aa-137">Response</span></span>
<span data-ttu-id="f66aa-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f66aa-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodsPolicy",
    "id": "authenticationMethodsPolicy",
    "displayName": "Authentication Methods Policy",
    "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
    "lastModifiedDateTime": "2021-05-24T18:02:30.5288302Z",
    "policyVersion": "1.4",
    "registrationEnforcement": {
        "authenticationMethodsRegistrationCampaign": {
            "snoozeDurationInDays": 2,
            "state": "enabled",
            "excludeTargets": [],
            "includeTargets": [
                {
                    "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                    "targetType": "group",
                    "targetedAuthenticationMethod": "microsoftAuthenticator"
                }
            ]
        }
    }
}
```
