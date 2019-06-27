---
title: 创建 identityProvider
description: 通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 identityProvider。
localization_priority: Normal
ms.openlocfilehash: 97a87d73090457a2e314a8b44903260b24e55a69
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262669"
---
# <a name="create-identityprovider"></a><span data-ttu-id="bf785-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="bf785-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf785-104">通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="bf785-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf785-105">权限</span><span class="sxs-lookup"><span data-stu-id="bf785-105">Permissions</span></span>

<span data-ttu-id="bf785-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf785-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf785-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf785-108">Permission type</span></span>      | <span data-ttu-id="bf785-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf785-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf785-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf785-110">Delegated (work or school account)</span></span>|<span data-ttu-id="bf785-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf785-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="bf785-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="bf785-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bf785-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf785-113">Not supported.</span></span>|
|<span data-ttu-id="bf785-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf785-114">Application</span></span>|<span data-ttu-id="bf785-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf785-115">Not supported.</span></span>|

<span data-ttu-id="bf785-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="bf785-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf785-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf785-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="bf785-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf785-118">Request headers</span></span>

|<span data-ttu-id="bf785-119">名称</span><span class="sxs-lookup"><span data-stu-id="bf785-119">Name</span></span>|<span data-ttu-id="bf785-120">说明</span><span class="sxs-lookup"><span data-stu-id="bf785-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bf785-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf785-121">Authorization</span></span>|<span data-ttu-id="bf785-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf785-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf785-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf785-124">Content-Type</span></span>|<span data-ttu-id="bf785-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf785-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf785-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf785-127">Request body</span></span>

<span data-ttu-id="bf785-128">在请求正文中，提供 [identityProvider](../resources/identityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf785-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="bf785-129">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="bf785-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="bf785-130">属性</span><span class="sxs-lookup"><span data-stu-id="bf785-130">Property</span></span>|<span data-ttu-id="bf785-131">类型</span><span class="sxs-lookup"><span data-stu-id="bf785-131">Type</span></span>|<span data-ttu-id="bf785-132">说明</span><span class="sxs-lookup"><span data-stu-id="bf785-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf785-133">clientId</span><span class="sxs-lookup"><span data-stu-id="bf785-133">clientId</span></span>|<span data-ttu-id="bf785-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bf785-134">String</span></span>|<span data-ttu-id="bf785-135">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="bf785-135">The client ID for the application.</span></span> <span data-ttu-id="bf785-136">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="bf785-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="bf785-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="bf785-137">clientSecret</span></span>|<span data-ttu-id="bf785-138">字符串</span><span class="sxs-lookup"><span data-stu-id="bf785-138">String</span></span>|<span data-ttu-id="bf785-139">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="bf785-139">The client secret for the application.</span></span> <span data-ttu-id="bf785-140">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="bf785-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="bf785-141">name</span><span class="sxs-lookup"><span data-stu-id="bf785-141">name</span></span>|<span data-ttu-id="bf785-142">字符串</span><span class="sxs-lookup"><span data-stu-id="bf785-142">String</span></span>|<span data-ttu-id="bf785-143">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bf785-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="bf785-144">type</span><span class="sxs-lookup"><span data-stu-id="bf785-144">type</span></span>|<span data-ttu-id="bf785-145">字符串</span><span class="sxs-lookup"><span data-stu-id="bf785-145">String</span></span>|<span data-ttu-id="bf785-146">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="bf785-146">The identity provider type.</span></span> <span data-ttu-id="bf785-147">它必须是下列值之一:</span><span class="sxs-lookup"><span data-stu-id="bf785-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="bf785-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="bf785-148">Microsoft</span></span><li/><span data-ttu-id="bf785-149">Google</span><span class="sxs-lookup"><span data-stu-id="bf785-149">Google</span></span><li/><span data-ttu-id="bf785-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="bf785-150">Amazon</span></span><li/><span data-ttu-id="bf785-151">领英</span><span class="sxs-lookup"><span data-stu-id="bf785-151">LinkedIn</span></span><li/><span data-ttu-id="bf785-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="bf785-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="bf785-153">响应</span><span class="sxs-lookup"><span data-stu-id="bf785-153">Response</span></span>

<span data-ttu-id="bf785-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [identityProvider](../resources/identityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf785-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="bf785-155">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf785-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="bf785-156">示例</span><span class="sxs-lookup"><span data-stu-id="bf785-156">Example</span></span>

<span data-ttu-id="bf785-157">以下示例会创建 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="bf785-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="bf785-158">请求</span><span class="sxs-lookup"><span data-stu-id="bf785-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="bf785-159">响应</span><span class="sxs-lookup"><span data-stu-id="bf785-159">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf785-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bf785-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf785-161">C#</span><span class="sxs-lookup"><span data-stu-id="bf785-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf785-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf785-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bf785-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="bf785-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
