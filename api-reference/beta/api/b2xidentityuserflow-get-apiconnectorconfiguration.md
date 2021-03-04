---
title: 获取 userFlowApiConnectorConfiguration
description: 获取 b2xIdentityUserFlow 的 userFlowApiConnectorConfiguration 属性。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 937e102e05b4b7e2a1b03538a0b023ae583ef3c6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438139"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="53d15-103">获取 userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="53d15-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="53d15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53d15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53d15-105">获取[b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md)中的[apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md)属性，以详细说明为用户流启用的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="53d15-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="53d15-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="53d15-106">Permissions</span></span>

<span data-ttu-id="53d15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d15-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53d15-109">Permission type</span></span>      | <span data-ttu-id="53d15-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53d15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d15-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53d15-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53d15-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53d15-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="53d15-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53d15-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="53d15-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53d15-114">Not supported.</span></span>|
|<span data-ttu-id="53d15-115">Application</span><span class="sxs-lookup"><span data-stu-id="53d15-115">Application</span></span>|<span data-ttu-id="53d15-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53d15-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="53d15-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="53d15-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="53d15-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="53d15-118">Global administrator</span></span>
* <span data-ttu-id="53d15-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="53d15-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="53d15-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53d15-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53d15-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53d15-121">Optional query parameters</span></span>

<span data-ttu-id="53d15-122">此方法支持 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53d15-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="53d15-123">例如，若要检索和步骤的 API `postFederationSignup` 连接器 `postAttributeCollection` ，请添加 `$expand=postFederationSignup,postAttributeCollection` 。</span><span class="sxs-lookup"><span data-stu-id="53d15-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="53d15-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="53d15-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="53d15-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="53d15-125">Request headers</span></span>

|<span data-ttu-id="53d15-126">名称</span><span class="sxs-lookup"><span data-stu-id="53d15-126">Name</span></span>|<span data-ttu-id="53d15-127">说明</span><span class="sxs-lookup"><span data-stu-id="53d15-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53d15-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="53d15-128">Authorization</span></span>|<span data-ttu-id="53d15-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53d15-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53d15-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="53d15-131">Request body</span></span>

<span data-ttu-id="53d15-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53d15-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d15-133">响应</span><span class="sxs-lookup"><span data-stu-id="53d15-133">Response</span></span>

<span data-ttu-id="53d15-134">如果成功，此方法将返回 `200 OK` 响应代码和 [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53d15-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="53d15-135">示例</span><span class="sxs-lookup"><span data-stu-id="53d15-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53d15-136">请求</span><span class="sxs-lookup"><span data-stu-id="53d15-136">Request</span></span>

<span data-ttu-id="53d15-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53d15-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53d15-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="53d15-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```
# <a name="c"></a>[<span data-ttu-id="53d15-139">C#</span><span class="sxs-lookup"><span data-stu-id="53d15-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-apiconnectorconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53d15-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53d15-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-apiconnectorconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53d15-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53d15-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-apiconnectorconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53d15-142">Java</span><span class="sxs-lookup"><span data-stu-id="53d15-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-apiconnectorconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53d15-143">响应</span><span class="sxs-lookup"><span data-stu-id="53d15-143">Response</span></span>

<span data-ttu-id="53d15-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53d15-144">The following is an example of the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration(postFederationSignup(),postAttributeCollection())",
    "postFederationSignup@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postFederationSignup/$entity",
    "postFederationSignup": {
        "id": "<guid1>",
        "displayName": "Test API Connector 1",
        "targetUrl": "https://someapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
        }
    },
    "postAttributeCollection@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postAttributeCollection/$entity",
    "postAttributeCollection": {
        "id": "<guid2>",
        "displayName": "Test API Connector 2",
        "targetUrl": "https://someotherapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME2>",
            "password": "******"
        }
    }
}
```
