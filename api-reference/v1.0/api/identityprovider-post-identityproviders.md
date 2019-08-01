---
title: 创建 identityProvider
description: 新建 identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ffd1f600395a1c72f2ab4c72ef1c3d3a358e387
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016151"
---
# <a name="create-identityprovider"></a><span data-ttu-id="80cec-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="80cec-103">Create identityProvider</span></span>

<span data-ttu-id="80cec-104">通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="80cec-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="80cec-105">权限</span><span class="sxs-lookup"><span data-stu-id="80cec-105">Permissions</span></span>

<span data-ttu-id="80cec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80cec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80cec-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="80cec-108">Permission type</span></span>      | <span data-ttu-id="80cec-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80cec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80cec-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80cec-110">Delegated (work or school account)</span></span>|<span data-ttu-id="80cec-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80cec-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="80cec-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="80cec-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="80cec-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="80cec-113">Not supported.</span></span>|
|<span data-ttu-id="80cec-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="80cec-114">Application</span></span>|<span data-ttu-id="80cec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80cec-115">Not supported.</span></span>|

<span data-ttu-id="80cec-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="80cec-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="80cec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80cec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="80cec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80cec-118">Request headers</span></span>

|<span data-ttu-id="80cec-119">名称</span><span class="sxs-lookup"><span data-stu-id="80cec-119">Name</span></span>|<span data-ttu-id="80cec-120">说明</span><span class="sxs-lookup"><span data-stu-id="80cec-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="80cec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80cec-121">Authorization</span></span>|<span data-ttu-id="80cec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80cec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="80cec-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80cec-124">Content-Type</span></span>|<span data-ttu-id="80cec-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="80cec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80cec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80cec-127">Request body</span></span>

<span data-ttu-id="80cec-128">在请求正文中，提供 [identityProvider](../resources/identityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80cec-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="80cec-129">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="80cec-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="80cec-130">属性</span><span class="sxs-lookup"><span data-stu-id="80cec-130">Property</span></span>|<span data-ttu-id="80cec-131">类型</span><span class="sxs-lookup"><span data-stu-id="80cec-131">Type</span></span>|<span data-ttu-id="80cec-132">说明</span><span class="sxs-lookup"><span data-stu-id="80cec-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80cec-133">clientId</span><span class="sxs-lookup"><span data-stu-id="80cec-133">clientId</span></span>|<span data-ttu-id="80cec-134">字符串</span><span class="sxs-lookup"><span data-stu-id="80cec-134">String</span></span>|<span data-ttu-id="80cec-135">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="80cec-135">The client ID for the application.</span></span> <span data-ttu-id="80cec-136">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="80cec-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="80cec-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="80cec-137">clientSecret</span></span>|<span data-ttu-id="80cec-138">字符串</span><span class="sxs-lookup"><span data-stu-id="80cec-138">String</span></span>|<span data-ttu-id="80cec-139">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="80cec-139">The client secret for the application.</span></span> <span data-ttu-id="80cec-140">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="80cec-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="80cec-141">name</span><span class="sxs-lookup"><span data-stu-id="80cec-141">name</span></span>|<span data-ttu-id="80cec-142">字符串</span><span class="sxs-lookup"><span data-stu-id="80cec-142">String</span></span>|<span data-ttu-id="80cec-143">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="80cec-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="80cec-144">type</span><span class="sxs-lookup"><span data-stu-id="80cec-144">type</span></span>|<span data-ttu-id="80cec-145">字符串</span><span class="sxs-lookup"><span data-stu-id="80cec-145">String</span></span>|<span data-ttu-id="80cec-146">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="80cec-146">The identity provider type.</span></span> <span data-ttu-id="80cec-147">它必须是 B2C 方案的下列值之一：</span><span class="sxs-lookup"><span data-stu-id="80cec-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="80cec-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="80cec-148">Microsoft</span></span><li/><span data-ttu-id="80cec-149">Google</span><span class="sxs-lookup"><span data-stu-id="80cec-149">Google</span></span><li/><span data-ttu-id="80cec-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="80cec-150">Amazon</span></span><li/><span data-ttu-id="80cec-151">领英</span><span class="sxs-lookup"><span data-stu-id="80cec-151">LinkedIn</span></span><li/><span data-ttu-id="80cec-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="80cec-152">Facebook</span></span><li/><span data-ttu-id="80cec-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="80cec-153">GitHub</span></span><li/><span data-ttu-id="80cec-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="80cec-154">Twitter</span></span><li/><span data-ttu-id="80cec-155">微博</span><span class="sxs-lookup"><span data-stu-id="80cec-155">Weibo</span></span><li/><span data-ttu-id="80cec-156">QQ</span><span class="sxs-lookup"><span data-stu-id="80cec-156">QQ</span></span><li/><span data-ttu-id="80cec-157">微信</span><span class="sxs-lookup"><span data-stu-id="80cec-157">WeChat</span></span></ul><span data-ttu-id="80cec-158">在 B2B 中，它只能是 Google</span><span class="sxs-lookup"><span data-stu-id="80cec-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="80cec-159">响应</span><span class="sxs-lookup"><span data-stu-id="80cec-159">Response</span></span>

<span data-ttu-id="80cec-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [identityProvider](../resources/identityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80cec-160">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="80cec-161">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="80cec-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="80cec-162">示例</span><span class="sxs-lookup"><span data-stu-id="80cec-162">Example</span></span>

<span data-ttu-id="80cec-163">以下示例会创建 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="80cec-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="80cec-164">请求</span><span class="sxs-lookup"><span data-stu-id="80cec-164">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="80cec-165">响应</span><span class="sxs-lookup"><span data-stu-id="80cec-165">Response</span></span>

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


