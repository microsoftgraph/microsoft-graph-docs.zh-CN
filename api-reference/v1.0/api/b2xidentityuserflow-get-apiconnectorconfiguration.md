---
title: 获取 userFlowApiConnectorConfiguration
description: 获取 b2xIdentityUserFlow 的 userFlowApiConnectorConfiguration 属性。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a9bdc99041265edf589a493ef5d83dc51f1c115a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882808"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="4630e-103">获取 userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="4630e-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="4630e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4630e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4630e-105">获取[b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md)中的[apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)属性，详细说明为用户流启用的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="4630e-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="4630e-106">权限</span><span class="sxs-lookup"><span data-stu-id="4630e-106">Permissions</span></span>

<span data-ttu-id="4630e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4630e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4630e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4630e-109">Permission type</span></span>      | <span data-ttu-id="4630e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4630e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4630e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4630e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4630e-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4630e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4630e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4630e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4630e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4630e-114">Not supported.</span></span>|
|<span data-ttu-id="4630e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4630e-115">Application</span></span>|<span data-ttu-id="4630e-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4630e-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4630e-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4630e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4630e-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4630e-118">Global administrator</span></span>
* <span data-ttu-id="4630e-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4630e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4630e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4630e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4630e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4630e-121">Optional query parameters</span></span>

<span data-ttu-id="4630e-122">此方法支持 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4630e-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="4630e-123">例如，若要检索 和 步骤的 API 连接器 `postFederationSignup` `postAttributeCollection` ，请添加 `$expand=postFederationSignup,postAttributeCollection` 。</span><span class="sxs-lookup"><span data-stu-id="4630e-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="4630e-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4630e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4630e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4630e-125">Request headers</span></span>

|<span data-ttu-id="4630e-126">名称</span><span class="sxs-lookup"><span data-stu-id="4630e-126">Name</span></span>|<span data-ttu-id="4630e-127">说明</span><span class="sxs-lookup"><span data-stu-id="4630e-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4630e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="4630e-128">Authorization</span></span>|<span data-ttu-id="4630e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4630e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4630e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4630e-131">Request body</span></span>

<span data-ttu-id="4630e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4630e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4630e-133">响应</span><span class="sxs-lookup"><span data-stu-id="4630e-133">Response</span></span>

<span data-ttu-id="4630e-134">如果成功，此方法返回 响应 `200 OK` 代码和 [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4630e-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="4630e-135">示例</span><span class="sxs-lookup"><span data-stu-id="4630e-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4630e-136">请求</span><span class="sxs-lookup"><span data-stu-id="4630e-136">Request</span></span>

<span data-ttu-id="4630e-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4630e-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```

### <a name="response"></a><span data-ttu-id="4630e-138">响应</span><span class="sxs-lookup"><span data-stu-id="4630e-138">Response</span></span>

<span data-ttu-id="4630e-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4630e-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration(postFederationSignup(),postAttributeCollection())",
    "postFederationSignup@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postFederationSignup/$entity",
    "postFederationSignup": {
        "id": "74d13179-2c02-4ae7-bff3-82842d4e2f1f",
        "displayName": "Test API Connector 1",
        "targetUrl": "https://someapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "apiAccount",
            "password": "******"
        }
    },
    "postAttributeCollection@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postAttributeCollection/$entity",
    "postAttributeCollection": {
        "id": "900bc92c-bcbf-4093-af8e-450a4a77635f",
        "displayName": "Test API Connector 2",
        "targetUrl": "https://someotherapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "apiAccount",
            "password": "******"
        }
    }
}
```
