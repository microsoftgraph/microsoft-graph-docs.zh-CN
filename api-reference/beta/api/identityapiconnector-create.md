---
title: 创建 identityApiConnector
description: 创建新的 identityApiConnector 对象。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e2ff03ae081a1d406a56c5a826664bb402983a4f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435611"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="a804e-103">创建 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="a804e-103">Create identityApiConnector</span></span>

<span data-ttu-id="a804e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a804e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a804e-105">创建新的 [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a804e-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a804e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a804e-106">Permissions</span></span>

<span data-ttu-id="a804e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a804e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a804e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a804e-109">Permission type</span></span>                        | <span data-ttu-id="a804e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a804e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a804e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a804e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a804e-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a804e-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="a804e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a804e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a804e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a804e-114">Not supported.</span></span>  |
| <span data-ttu-id="a804e-115">Application</span><span class="sxs-lookup"><span data-stu-id="a804e-115">Application</span></span>                            | <span data-ttu-id="a804e-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a804e-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="a804e-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="a804e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a804e-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a804e-118">Global administrator</span></span>
* <span data-ttu-id="a804e-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="a804e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a804e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a804e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="a804e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a804e-121">Request headers</span></span>

| <span data-ttu-id="a804e-122">名称</span><span class="sxs-lookup"><span data-stu-id="a804e-122">Name</span></span>          | <span data-ttu-id="a804e-123">说明</span><span class="sxs-lookup"><span data-stu-id="a804e-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="a804e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a804e-124">Authorization</span></span> | <span data-ttu-id="a804e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a804e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a804e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a804e-127">Content-Type</span></span>  | <span data-ttu-id="a804e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a804e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a804e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a804e-130">Request body</span></span>

<span data-ttu-id="a804e-131">在请求正文中，提供 [identityApiConnector](../resources/identityapiconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a804e-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="a804e-132">下表显示创建 [identityApiConnector 时所需的属性](../resources/identityapiconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="a804e-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="a804e-133">属性</span><span class="sxs-lookup"><span data-stu-id="a804e-133">Property</span></span>|<span data-ttu-id="a804e-134">类型</span><span class="sxs-lookup"><span data-stu-id="a804e-134">Type</span></span>|<span data-ttu-id="a804e-135">说明</span><span class="sxs-lookup"><span data-stu-id="a804e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a804e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a804e-136">displayName</span></span>|<span data-ttu-id="a804e-137">String</span><span class="sxs-lookup"><span data-stu-id="a804e-137">String</span></span>| <span data-ttu-id="a804e-138">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="a804e-138">The name of the API connector.</span></span> |
|<span data-ttu-id="a804e-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="a804e-139">targetUrl</span></span>|<span data-ttu-id="a804e-140">String</span><span class="sxs-lookup"><span data-stu-id="a804e-140">String</span></span>| <span data-ttu-id="a804e-141">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="a804e-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="a804e-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a804e-142">authenticationConfiguration</span></span>|[<span data-ttu-id="a804e-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="a804e-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="a804e-144">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="a804e-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="a804e-145">仅 [支持基本](../resources/basicauthentication.md) 身份验证。</span><span class="sxs-lookup"><span data-stu-id="a804e-145">Only [Basic authentication](../resources/basicauthentication.md) is supported.</span></span>|

## <a name="response"></a><span data-ttu-id="a804e-146">响应</span><span class="sxs-lookup"><span data-stu-id="a804e-146">Response</span></span>

<span data-ttu-id="a804e-147">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a804e-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a804e-148">示例</span><span class="sxs-lookup"><span data-stu-id="a804e-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a804e-149">请求</span><span class="sxs-lookup"><span data-stu-id="a804e-149">Request</span></span>

<span data-ttu-id="a804e-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a804e-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a804e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a804e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username":"<USERNAME>",
      "password":"<PASSWORD>"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="a804e-152">C#</span><span class="sxs-lookup"><span data-stu-id="a804e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a804e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a804e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a804e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a804e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a804e-155">Java</span><span class="sxs-lookup"><span data-stu-id="a804e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a804e-156">响应</span><span class="sxs-lookup"><span data-stu-id="a804e-156">Response</span></span>

<span data-ttu-id="a804e-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a804e-157">The following is an example of the response.</span></span>

<span data-ttu-id="a804e-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a804e-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
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
