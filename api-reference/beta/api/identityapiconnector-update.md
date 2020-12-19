---
title: 更新 identityApiConnector
description: 更新 identityApiConnector 对象的属性。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e06927b3058f78396d9df6d54e7336ff6ba1b521
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720148"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="7be09-103">更新 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7be09-103">Update identityApiConnector</span></span>

<span data-ttu-id="7be09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be09-105">更新 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="7be09-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7be09-106">权限</span><span class="sxs-lookup"><span data-stu-id="7be09-106">Permissions</span></span>

<span data-ttu-id="7be09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7be09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7be09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7be09-109">Permission type</span></span>                        | <span data-ttu-id="7be09-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7be09-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7be09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7be09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7be09-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be09-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="7be09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7be09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7be09-114">Not supported.</span></span>  |
| <span data-ttu-id="7be09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7be09-115">Application</span></span>                            | <span data-ttu-id="7be09-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be09-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="7be09-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="7be09-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7be09-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7be09-118">Global administrator</span></span>
* <span data-ttu-id="7be09-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="7be09-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7be09-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7be09-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="7be09-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7be09-121">Request headers</span></span>
|<span data-ttu-id="7be09-122">名称</span><span class="sxs-lookup"><span data-stu-id="7be09-122">Name</span></span>|<span data-ttu-id="7be09-123">说明</span><span class="sxs-lookup"><span data-stu-id="7be09-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7be09-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7be09-124">Authorization</span></span>|<span data-ttu-id="7be09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7be09-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7be09-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7be09-127">Content-Type</span></span>|<span data-ttu-id="7be09-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7be09-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7be09-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7be09-130">Request body</span></span>
<span data-ttu-id="7be09-131">在请求正文中，提供 [identityApiConnector](../resources/identityapiconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7be09-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="7be09-132">下表显示了可以更新 [的 identityApiConnector](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="7be09-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="7be09-133">属性</span><span class="sxs-lookup"><span data-stu-id="7be09-133">Property</span></span>|<span data-ttu-id="7be09-134">类型</span><span class="sxs-lookup"><span data-stu-id="7be09-134">Type</span></span>|<span data-ttu-id="7be09-135">说明</span><span class="sxs-lookup"><span data-stu-id="7be09-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be09-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7be09-136">displayName</span></span>|<span data-ttu-id="7be09-137">String</span><span class="sxs-lookup"><span data-stu-id="7be09-137">String</span></span>| <span data-ttu-id="7be09-138">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="7be09-138">The name of the API connector.</span></span> |
|<span data-ttu-id="7be09-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="7be09-139">targetUrl</span></span>|<span data-ttu-id="7be09-140">String</span><span class="sxs-lookup"><span data-stu-id="7be09-140">String</span></span>| <span data-ttu-id="7be09-141">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="7be09-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="7be09-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7be09-142">authenticationConfiguration</span></span>|[<span data-ttu-id="7be09-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="7be09-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="7be09-144">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="7be09-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="7be09-145">目前 [仅](../resources/basicauthentication.md) 支持基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="7be09-145">Only [Basic authentication](../resources/basicauthentication.md) is supported at this time.</span></span> <span data-ttu-id="7be09-146">apiAuthenticationConfigurationBase 的所有属性必须同时设置，如用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="7be09-146">All properties of the apiAuthenticationConfigurationBase must be set at the same time, like both username and password.</span></span>|

## <a name="response"></a><span data-ttu-id="7be09-147">响应</span><span class="sxs-lookup"><span data-stu-id="7be09-147">Response</span></span>

<span data-ttu-id="7be09-148">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7be09-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7be09-149">示例</span><span class="sxs-lookup"><span data-stu-id="7be09-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7be09-150">请求</span><span class="sxs-lookup"><span data-stu-id="7be09-150">Request</span></span>

<span data-ttu-id="7be09-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7be09-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "displayName": "New Test API",
  "targetUrl": "https://otherapi.com/api/endpoint",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.basicAuthentication",
    "username":"<NEW_USERNAME>", 
    "password":"<NEW_PASSWORD>"
  }
}
```

### <a name="response"></a><span data-ttu-id="7be09-152">响应</span><span class="sxs-lookup"><span data-stu-id="7be09-152">Response</span></span>

<span data-ttu-id="7be09-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7be09-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
