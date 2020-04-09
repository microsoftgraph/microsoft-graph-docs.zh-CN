---
title: 创建 identityProvider
description: 通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 540af7a9ebb9ea56f6f3f61cff89ff6a4d3973d6
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199590"
---
# <a name="create-identityprovider"></a><span data-ttu-id="c7d0e-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="c7d0e-103">Create identityProvider</span></span>

<span data-ttu-id="c7d0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7d0e-105">通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-105">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7d0e-106">权限</span><span class="sxs-lookup"><span data-stu-id="c7d0e-106">Permissions</span></span>

<span data-ttu-id="c7d0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7d0e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7d0e-109">Permission type</span></span>      | <span data-ttu-id="c7d0e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7d0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7d0e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7d0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d0e-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d0e-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c7d0e-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="c7d0e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c7d0e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-114">Not supported.</span></span>|
|<span data-ttu-id="c7d0e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7d0e-115">Application</span></span>|<span data-ttu-id="c7d0e-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d0e-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="c7d0e-117">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7d0e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7d0e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c7d0e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7d0e-119">Request headers</span></span>

|<span data-ttu-id="c7d0e-120">名称</span><span class="sxs-lookup"><span data-stu-id="c7d0e-120">Name</span></span>|<span data-ttu-id="c7d0e-121">说明</span><span class="sxs-lookup"><span data-stu-id="c7d0e-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c7d0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7d0e-122">Authorization</span></span>|<span data-ttu-id="c7d0e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7d0e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7d0e-125">Content-Type</span></span>|<span data-ttu-id="c7d0e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c7d0e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d0e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7d0e-128">Request body</span></span>

<span data-ttu-id="c7d0e-129">在请求正文中，提供 [identityProvider](../resources/identityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-129">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="c7d0e-130">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-130">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="c7d0e-131">属性</span><span class="sxs-lookup"><span data-stu-id="c7d0e-131">Property</span></span>|<span data-ttu-id="c7d0e-132">类型</span><span class="sxs-lookup"><span data-stu-id="c7d0e-132">Type</span></span>|<span data-ttu-id="c7d0e-133">说明</span><span class="sxs-lookup"><span data-stu-id="c7d0e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7d0e-134">clientId</span><span class="sxs-lookup"><span data-stu-id="c7d0e-134">clientId</span></span>|<span data-ttu-id="c7d0e-135">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d0e-135">String</span></span>|<span data-ttu-id="c7d0e-136">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-136">The client ID for the application.</span></span> <span data-ttu-id="c7d0e-137">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c7d0e-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="c7d0e-138">clientSecret</span></span>|<span data-ttu-id="c7d0e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d0e-139">String</span></span>|<span data-ttu-id="c7d0e-140">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-140">The client secret for the application.</span></span> <span data-ttu-id="c7d0e-141">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c7d0e-142">name</span><span class="sxs-lookup"><span data-stu-id="c7d0e-142">name</span></span>|<span data-ttu-id="c7d0e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d0e-143">String</span></span>|<span data-ttu-id="c7d0e-144">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-144">The display name of the identity provider.</span></span>|
|<span data-ttu-id="c7d0e-145">type</span><span class="sxs-lookup"><span data-stu-id="c7d0e-145">type</span></span>|<span data-ttu-id="c7d0e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d0e-146">String</span></span>|<span data-ttu-id="c7d0e-147">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-147">The identity provider type.</span></span> <span data-ttu-id="c7d0e-148">它必须是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="c7d0e-148">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="c7d0e-149">Microsoft</span><span class="sxs-lookup"><span data-stu-id="c7d0e-149">Microsoft</span></span><li/><span data-ttu-id="c7d0e-150">Google</span><span class="sxs-lookup"><span data-stu-id="c7d0e-150">Google</span></span><li/><span data-ttu-id="c7d0e-151">Amazon</span><span class="sxs-lookup"><span data-stu-id="c7d0e-151">Amazon</span></span><li/><span data-ttu-id="c7d0e-152">领英</span><span class="sxs-lookup"><span data-stu-id="c7d0e-152">LinkedIn</span></span><li/><span data-ttu-id="c7d0e-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="c7d0e-153">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="c7d0e-154">响应</span><span class="sxs-lookup"><span data-stu-id="c7d0e-154">Response</span></span>

<span data-ttu-id="c7d0e-155">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [identityProvider](../resources/identityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-155">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="c7d0e-156">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="c7d0e-157">示例</span><span class="sxs-lookup"><span data-stu-id="c7d0e-157">Example</span></span>

<span data-ttu-id="c7d0e-158">以下示例会创建 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="c7d0e-158">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="c7d0e-159">请求</span><span class="sxs-lookup"><span data-stu-id="c7d0e-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c7d0e-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d0e-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c7d0e-161">C#</span><span class="sxs-lookup"><span data-stu-id="c7d0e-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7d0e-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7d0e-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7d0e-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7d0e-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c7d0e-164">响应</span><span class="sxs-lookup"><span data-stu-id="c7d0e-164">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
