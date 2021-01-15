---
title: 获取 identityApiConnector
description: 读取 API 连接器的属性。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: faadb04acd2768905a3ecdd8a3d3723cb55b9d11
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873673"
---
# <a name="get-identityapiconnector"></a><span data-ttu-id="0ac90-103">获取 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="0ac90-103">Get identityApiConnector</span></span>

<span data-ttu-id="0ac90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ac90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ac90-105">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0ac90-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac90-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ac90-106">Permissions</span></span>

<span data-ttu-id="0ac90-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ac90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ac90-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ac90-109">Permission type</span></span>                        | <span data-ttu-id="0ac90-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ac90-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="0ac90-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ac90-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac90-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="0ac90-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac90-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac90-114">Not supported.</span></span>  |
| <span data-ttu-id="0ac90-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ac90-115">Application</span></span>                            | <span data-ttu-id="0ac90-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac90-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="0ac90-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="0ac90-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0ac90-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0ac90-118">Global administrator</span></span>
* <span data-ttu-id="0ac90-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="0ac90-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0ac90-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ac90-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ac90-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ac90-121">Optional query parameters</span></span>
<span data-ttu-id="0ac90-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ac90-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0ac90-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0ac90-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ac90-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ac90-124">Request headers</span></span>
|<span data-ttu-id="0ac90-125">名称</span><span class="sxs-lookup"><span data-stu-id="0ac90-125">Name</span></span>|<span data-ttu-id="0ac90-126">说明</span><span class="sxs-lookup"><span data-stu-id="0ac90-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ac90-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac90-127">Authorization</span></span>|<span data-ttu-id="0ac90-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ac90-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac90-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ac90-130">Request body</span></span>
<span data-ttu-id="0ac90-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ac90-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ac90-132">响应</span><span class="sxs-lookup"><span data-stu-id="0ac90-132">Response</span></span>

<span data-ttu-id="0ac90-133">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ac90-133">If successful, this method returns a `200 OK` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ac90-134">示例</span><span class="sxs-lookup"><span data-stu-id="0ac90-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ac90-135">请求</span><span class="sxs-lookup"><span data-stu-id="0ac90-135">Request</span></span>

<span data-ttu-id="0ac90-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ac90-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ac90-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac90-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityapiconnector"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="0ac90-138">C#</span><span class="sxs-lookup"><span data-stu-id="0ac90-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ac90-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ac90-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ac90-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ac90-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ac90-141">Java</span><span class="sxs-lookup"><span data-stu-id="0ac90-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ac90-142">响应</span><span class="sxs-lookup"><span data-stu-id="0ac90-142">Response</span></span>

<span data-ttu-id="0ac90-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ac90-143">The following is an example of the response.</span></span>

<span data-ttu-id="0ac90-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ac90-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
