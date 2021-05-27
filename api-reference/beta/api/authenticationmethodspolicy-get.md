---
title: 获取 authenticationMethodsPolicy
description: 读取 authenticationMethodsPolicy 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b54b95f3db35d744d400fb50a221cdfdad12890b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682874"
---
# <a name="get-authenticationmethodspolicy"></a><span data-ttu-id="60344-103">获取 authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="60344-103">Get authenticationMethodsPolicy</span></span>
<span data-ttu-id="60344-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60344-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60344-105">读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60344-105">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60344-106">权限</span><span class="sxs-lookup"><span data-stu-id="60344-106">Permissions</span></span>
<span data-ttu-id="60344-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60344-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60344-109">Permission type</span></span>|<span data-ttu-id="60344-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60344-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60344-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60344-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60344-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="60344-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="60344-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60344-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60344-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="60344-114">Not supported.</span></span>|
|<span data-ttu-id="60344-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="60344-115">Application</span></span>|<span data-ttu-id="60344-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="60344-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="60344-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60344-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60344-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="60344-118">Optional query parameters</span></span>
<span data-ttu-id="60344-119">此方法不支持任何可选的查询参数。</span><span class="sxs-lookup"><span data-stu-id="60344-119">This method does not support any optional query parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60344-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60344-120">Request headers</span></span>
|<span data-ttu-id="60344-121">名称</span><span class="sxs-lookup"><span data-stu-id="60344-121">Name</span></span>|<span data-ttu-id="60344-122">说明</span><span class="sxs-lookup"><span data-stu-id="60344-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60344-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60344-123">Authorization</span></span>|<span data-ttu-id="60344-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60344-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60344-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="60344-126">Request body</span></span>
<span data-ttu-id="60344-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60344-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60344-128">响应</span><span class="sxs-lookup"><span data-stu-id="60344-128">Response</span></span>

<span data-ttu-id="60344-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60344-129">If successful, this method returns a `200 OK` response code and an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60344-130">示例</span><span class="sxs-lookup"><span data-stu-id="60344-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60344-131">请求</span><span class="sxs-lookup"><span data-stu-id="60344-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```


### <a name="response"></a><span data-ttu-id="60344-132">响应</span><span class="sxs-lookup"><span data-stu-id="60344-132">Response</span></span>
<span data-ttu-id="60344-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="60344-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
