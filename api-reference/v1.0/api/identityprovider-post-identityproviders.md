---
title: 创建 identityProvider
description: 新建 identityProvider
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1e5e0a13b0518fc734f1c2d8d1fd40fa41833f71
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434242"
---
# <a name="create-identityprovider"></a><span data-ttu-id="8cca4-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="8cca4-103">Create identityProvider</span></span>

<span data-ttu-id="8cca4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cca4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cca4-105">通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="8cca4-105">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cca4-106">权限</span><span class="sxs-lookup"><span data-stu-id="8cca4-106">Permissions</span></span>

<span data-ttu-id="8cca4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cca4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cca4-109">Permission type</span></span>      | <span data-ttu-id="8cca4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cca4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cca4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cca4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cca4-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cca4-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="8cca4-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="8cca4-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8cca4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cca4-114">Not supported.</span></span>|
|<span data-ttu-id="8cca4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cca4-115">Application</span></span>|<span data-ttu-id="8cca4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cca4-116">Not supported.</span></span>|

<span data-ttu-id="8cca4-117">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="8cca4-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="8cca4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cca4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="8cca4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cca4-119">Request headers</span></span>

|<span data-ttu-id="8cca4-120">名称</span><span class="sxs-lookup"><span data-stu-id="8cca4-120">Name</span></span>|<span data-ttu-id="8cca4-121">说明</span><span class="sxs-lookup"><span data-stu-id="8cca4-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8cca4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cca4-122">Authorization</span></span>|<span data-ttu-id="8cca4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cca4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8cca4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cca4-125">Content-Type</span></span>|<span data-ttu-id="8cca4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8cca4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cca4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cca4-128">Request body</span></span>

<span data-ttu-id="8cca4-129">在请求正文中，提供 [identityProvider](../resources/identityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cca4-129">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="8cca4-130">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="8cca4-130">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="8cca4-131">属性</span><span class="sxs-lookup"><span data-stu-id="8cca4-131">Property</span></span>|<span data-ttu-id="8cca4-132">类型</span><span class="sxs-lookup"><span data-stu-id="8cca4-132">Type</span></span>|<span data-ttu-id="8cca4-133">说明</span><span class="sxs-lookup"><span data-stu-id="8cca4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cca4-134">clientId</span><span class="sxs-lookup"><span data-stu-id="8cca4-134">clientId</span></span>|<span data-ttu-id="8cca4-135">字符串</span><span class="sxs-lookup"><span data-stu-id="8cca4-135">String</span></span>|<span data-ttu-id="8cca4-136">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="8cca4-136">The client ID for the application.</span></span> <span data-ttu-id="8cca4-137">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="8cca4-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="8cca4-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="8cca4-138">clientSecret</span></span>|<span data-ttu-id="8cca4-139">字符串</span><span class="sxs-lookup"><span data-stu-id="8cca4-139">String</span></span>|<span data-ttu-id="8cca4-140">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="8cca4-140">The client secret for the application.</span></span> <span data-ttu-id="8cca4-141">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="8cca4-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="8cca4-142">name</span><span class="sxs-lookup"><span data-stu-id="8cca4-142">name</span></span>|<span data-ttu-id="8cca4-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8cca4-143">String</span></span>|<span data-ttu-id="8cca4-144">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8cca4-144">The display name of the identity provider.</span></span>|
|<span data-ttu-id="8cca4-145">type</span><span class="sxs-lookup"><span data-stu-id="8cca4-145">type</span></span>|<span data-ttu-id="8cca4-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8cca4-146">String</span></span>|<span data-ttu-id="8cca4-147">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="8cca4-147">The identity provider type.</span></span> <span data-ttu-id="8cca4-148">它必须是 B2C 方案的下列值之一：</span><span class="sxs-lookup"><span data-stu-id="8cca4-148">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="8cca4-149">Microsoft</span><span class="sxs-lookup"><span data-stu-id="8cca4-149">Microsoft</span></span><li/><span data-ttu-id="8cca4-150">Google</span><span class="sxs-lookup"><span data-stu-id="8cca4-150">Google</span></span><li/><span data-ttu-id="8cca4-151">Amazon</span><span class="sxs-lookup"><span data-stu-id="8cca4-151">Amazon</span></span><li/><span data-ttu-id="8cca4-152">领英</span><span class="sxs-lookup"><span data-stu-id="8cca4-152">LinkedIn</span></span><li/><span data-ttu-id="8cca4-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="8cca4-153">Facebook</span></span><li/><span data-ttu-id="8cca4-154">GitHub</span><span class="sxs-lookup"><span data-stu-id="8cca4-154">GitHub</span></span><li/><span data-ttu-id="8cca4-155">Twitter</span><span class="sxs-lookup"><span data-stu-id="8cca4-155">Twitter</span></span><li/><span data-ttu-id="8cca4-156">微博</span><span class="sxs-lookup"><span data-stu-id="8cca4-156">Weibo</span></span><li/><span data-ttu-id="8cca4-157">QQ</span><span class="sxs-lookup"><span data-stu-id="8cca4-157">QQ</span></span><li/><span data-ttu-id="8cca4-158">微信</span><span class="sxs-lookup"><span data-stu-id="8cca4-158">WeChat</span></span></ul><span data-ttu-id="8cca4-159">在 B2B 中，它只能是 Google</span><span class="sxs-lookup"><span data-stu-id="8cca4-159">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="8cca4-160">响应</span><span class="sxs-lookup"><span data-stu-id="8cca4-160">Response</span></span>

<span data-ttu-id="8cca4-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [identityProvider](../resources/identityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8cca4-161">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="8cca4-162">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="8cca4-162">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="8cca4-163">示例</span><span class="sxs-lookup"><span data-stu-id="8cca4-163">Example</span></span>

<span data-ttu-id="8cca4-164">以下示例会创建 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="8cca4-164">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="8cca4-165">请求</span><span class="sxs-lookup"><span data-stu-id="8cca4-165">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="8cca4-166">响应</span><span class="sxs-lookup"><span data-stu-id="8cca4-166">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



