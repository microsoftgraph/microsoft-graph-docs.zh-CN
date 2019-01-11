---
title: 创建 identityProvider
description: 通过指定显示名称、 identityProvider 类型、 客户端 ID 和客户端机密创建新 identityProvider。
localization_priority: Normal
ms.openlocfilehash: 50ead5acbbda7725e44de55865d6fe2184c89647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866232"
---
# <a name="create-identityprovider"></a><span data-ttu-id="c8bbd-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="c8bbd-103">Create identityProvider</span></span>

> <span data-ttu-id="c8bbd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8bbd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8bbd-106">通过指定显示名称、 identityProvider 类型、 客户端 ID 和客户端机密创建新[identityProvider](../resources/identityprovider.md) 。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-106">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8bbd-107">权限</span><span class="sxs-lookup"><span data-stu-id="c8bbd-107">Permissions</span></span>

<span data-ttu-id="c8bbd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8bbd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8bbd-110">Permission type</span></span>      | <span data-ttu-id="c8bbd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8bbd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8bbd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8bbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8bbd-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8bbd-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c8bbd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8bbd-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c8bbd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-115">Not supported.</span></span>|
|<span data-ttu-id="c8bbd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8bbd-116">Application</span></span>|<span data-ttu-id="c8bbd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-117">Not supported.</span></span>|

<span data-ttu-id="c8bbd-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c8bbd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8bbd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c8bbd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8bbd-120">Request headers</span></span>

|<span data-ttu-id="c8bbd-121">名称</span><span class="sxs-lookup"><span data-stu-id="c8bbd-121">Name</span></span>|<span data-ttu-id="c8bbd-122">说明</span><span class="sxs-lookup"><span data-stu-id="c8bbd-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c8bbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8bbd-123">Authorization</span></span>|<span data-ttu-id="c8bbd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c8bbd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8bbd-126">Content-Type</span></span>|<span data-ttu-id="c8bbd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c8bbd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8bbd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8bbd-129">Request body</span></span>

<span data-ttu-id="c8bbd-130">在请求正文中，提供[identityProvider](../resources/identityprovider.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-130">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="c8bbd-131">下表中列出的所有属性都是必需的。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-131">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="c8bbd-132">属性</span><span class="sxs-lookup"><span data-stu-id="c8bbd-132">Property</span></span>|<span data-ttu-id="c8bbd-133">类型</span><span class="sxs-lookup"><span data-stu-id="c8bbd-133">Type</span></span>|<span data-ttu-id="c8bbd-134">Description</span><span class="sxs-lookup"><span data-stu-id="c8bbd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8bbd-135">clientId</span><span class="sxs-lookup"><span data-stu-id="c8bbd-135">clientId</span></span>|<span data-ttu-id="c8bbd-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c8bbd-136">String</span></span>|<span data-ttu-id="c8bbd-137">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-137">The client ID for the application.</span></span> <span data-ttu-id="c8bbd-138">这是注册的标识提供程序的应用程序时所获得的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-138">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c8bbd-139">clientSecret</span><span class="sxs-lookup"><span data-stu-id="c8bbd-139">clientSecret</span></span>|<span data-ttu-id="c8bbd-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c8bbd-140">String</span></span>|<span data-ttu-id="c8bbd-141">应用程序客户端机密。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-141">The client secret for the application.</span></span> <span data-ttu-id="c8bbd-142">这是注册的标识提供程序的应用程序时所获得的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-142">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c8bbd-143">name</span><span class="sxs-lookup"><span data-stu-id="c8bbd-143">name</span></span>|<span data-ttu-id="c8bbd-144">字符串</span><span class="sxs-lookup"><span data-stu-id="c8bbd-144">String</span></span>|<span data-ttu-id="c8bbd-145">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-145">The display name of the identity provider.</span></span>|
|<span data-ttu-id="c8bbd-146">type</span><span class="sxs-lookup"><span data-stu-id="c8bbd-146">type</span></span>|<span data-ttu-id="c8bbd-147">字符串</span><span class="sxs-lookup"><span data-stu-id="c8bbd-147">String</span></span>|<span data-ttu-id="c8bbd-148">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-148">The identity provider type.</span></span> <span data-ttu-id="c8bbd-149">它必须是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="c8bbd-149">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="c8bbd-150">Microsoft</span><span class="sxs-lookup"><span data-stu-id="c8bbd-150">Microsoft</span></span><li/><span data-ttu-id="c8bbd-151">Google</span><span class="sxs-lookup"><span data-stu-id="c8bbd-151">Google</span></span><li/><span data-ttu-id="c8bbd-152">Amazon</span><span class="sxs-lookup"><span data-stu-id="c8bbd-152">Amazon</span></span><li/><span data-ttu-id="c8bbd-153">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="c8bbd-153">LinkedIn</span></span><li/><span data-ttu-id="c8bbd-154">Facebook</span><span class="sxs-lookup"><span data-stu-id="c8bbd-154">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="c8bbd-155">响应</span><span class="sxs-lookup"><span data-stu-id="c8bbd-155">Response</span></span>

<span data-ttu-id="c8bbd-156">如果成功，此方法返回`201 Created`响应正文中的响应代码和[identityProvider](../resources/identityprovider.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-156">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="c8bbd-157">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-157">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="c8bbd-158">示例</span><span class="sxs-lookup"><span data-stu-id="c8bbd-158">Example</span></span>

<span data-ttu-id="c8bbd-159">下面的示例创建**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="c8bbd-159">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="c8bbd-160">请求</span><span class="sxs-lookup"><span data-stu-id="c8bbd-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="c8bbd-161">响应</span><span class="sxs-lookup"><span data-stu-id="c8bbd-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
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
