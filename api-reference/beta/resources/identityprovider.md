---
title: identityProvider 资源类型
description: 代表 Azure Active Directory (Azure AD) 标识提供程序。 Microsoft、 Google、 Facebook、 Amazon 或 LinkedIn，可以是标识提供程序。
localization_priority: Normal
ms.openlocfilehash: afd21635d932582f2a9ee6c2cde1cf45a9d4260f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511616"
---
# <a name="identityprovider-resource-type"></a><span data-ttu-id="d249c-104">identityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="d249c-104">identityProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d249c-105">代表 Azure Active Directory (Azure AD) 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d249c-105">Represents an Azure Active Directory (Azure AD) identity provider.</span></span> <span data-ttu-id="d249c-106">Microsoft、 Google、 Facebook、 Amazon 或 LinkedIn，可以是标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d249c-106">The identity provider can be Microsoft, Google, Facebook, Amazon, or LinkedIn.</span></span>

<span data-ttu-id="d249c-107">Azure AD B2C 租户中配置的身份提供程序支持：</span><span class="sxs-lookup"><span data-stu-id="d249c-107">Configuring an identity provider in your Azure AD B2C tenant enables:</span></span>

* <span data-ttu-id="d249c-108">用户注册并使用目标应用程序中的社交帐户登录。</span><span class="sxs-lookup"><span data-stu-id="d249c-108">Users to sign up and sign in using a social account in a consumer application.</span></span> <span data-ttu-id="d249c-109">例如，应用程序可以使用 Azure AD B2C 允许用户使用 Facebook 帐户对服务注册。</span><span class="sxs-lookup"><span data-stu-id="d249c-109">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account.</span></span>
* <span data-ttu-id="d249c-110">用户链接现有的本地帐户向使用者应用程序中的社交帐户。</span><span class="sxs-lookup"><span data-stu-id="d249c-110">Users to link an existing local account to a social account in a consumer application.</span></span> <span data-ttu-id="d249c-111">例如，用户已创建的用户名和密码 （本地帐户） 的应用程序中。</span><span class="sxs-lookup"><span data-stu-id="d249c-111">For example, a user has created a username and password (local account) in the application.</span></span> <span data-ttu-id="d249c-112">更高版本用户决定将现有的本地帐户链接到其 Facebook 帐户，以便他们可以使用 Facebook 登录。</span><span class="sxs-lookup"><span data-stu-id="d249c-112">The user later decides to link the existing local account to their Facebook account so they can sign in using Facebook.</span></span>

<span data-ttu-id="d249c-113">Azure AD 租户中配置的身份提供程序使未来 B2B 来宾方案。</span><span class="sxs-lookup"><span data-stu-id="d249c-113">Configuring an identity provider in your Azure AD tenant enables future B2B guest scenarios.</span></span> <span data-ttu-id="d249c-114">例如，组织有需要与 Gmail 用户共享的 Office 365 中的资源。</span><span class="sxs-lookup"><span data-stu-id="d249c-114">For example, an organization has resources in Office 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="d249c-115">Gmail 用户将使用其 Google 帐户凭据进行身份验证和访问的文档。</span><span class="sxs-lookup"><span data-stu-id="d249c-115">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

## <a name="methods"></a><span data-ttu-id="d249c-116">方法</span><span class="sxs-lookup"><span data-stu-id="d249c-116">Methods</span></span>

| <span data-ttu-id="d249c-117">方法</span><span class="sxs-lookup"><span data-stu-id="d249c-117">Method</span></span>       | <span data-ttu-id="d249c-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="d249c-118">Return Type</span></span>  |<span data-ttu-id="d249c-119">说明</span><span class="sxs-lookup"><span data-stu-id="d249c-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d249c-120">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="d249c-120">Get identityProvider</span></span>](../api/identityprovider-get.md) |<span data-ttu-id="d249c-121">identityProvider</span><span class="sxs-lookup"><span data-stu-id="d249c-121">identityProvider</span></span>|<span data-ttu-id="d249c-122">读取的现有 identityProvider 属性。</span><span class="sxs-lookup"><span data-stu-id="d249c-122">Read properties of an existing identityProvider.</span></span>|
|[<span data-ttu-id="d249c-123">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="d249c-123">Create identityProvider</span></span>](../api/identityprovider-post-identityproviders.md)|<span data-ttu-id="d249c-124">identityProvider</span><span class="sxs-lookup"><span data-stu-id="d249c-124">identityProvider</span></span>|<span data-ttu-id="d249c-125">创建新 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="d249c-125">Create a new identityProvider.</span></span>|
|[<span data-ttu-id="d249c-126">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="d249c-126">Update identityProvider</span></span>](../api/identityprovider-update.md)|<span data-ttu-id="d249c-127">无</span><span class="sxs-lookup"><span data-stu-id="d249c-127">None</span></span>|<span data-ttu-id="d249c-128">更新现有 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="d249c-128">Update an existing identityProvider.</span></span>|
|[<span data-ttu-id="d249c-129">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="d249c-129">Delete identityProvider</span></span>](../api/identityprovider-delete.md)|<span data-ttu-id="d249c-130">无</span><span class="sxs-lookup"><span data-stu-id="d249c-130">None</span></span>|<span data-ttu-id="d249c-131">删除现有 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="d249c-131">Delete an existing identityProvider.</span></span>|
|[<span data-ttu-id="d249c-132">列表 identityProviders</span><span class="sxs-lookup"><span data-stu-id="d249c-132">List identityProviders</span></span>](../api/identityprovider-list.md)|<span data-ttu-id="d249c-133">identityProvider 集合</span><span class="sxs-lookup"><span data-stu-id="d249c-133">identityProvider collection</span></span>|<span data-ttu-id="d249c-134">列出所有 identityProviders 配置租户中。</span><span class="sxs-lookup"><span data-stu-id="d249c-134">List all identityProviders configured in a tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="d249c-135">属性</span><span class="sxs-lookup"><span data-stu-id="d249c-135">Properties</span></span>

|<span data-ttu-id="d249c-136">属性</span><span class="sxs-lookup"><span data-stu-id="d249c-136">Property</span></span>|<span data-ttu-id="d249c-137">类型</span><span class="sxs-lookup"><span data-stu-id="d249c-137">Type</span></span>|<span data-ttu-id="d249c-138">必需</span><span class="sxs-lookup"><span data-stu-id="d249c-138">Required</span></span>|<span data-ttu-id="d249c-139">可为 Null</span><span class="sxs-lookup"><span data-stu-id="d249c-139">Nullable</span></span>|<span data-ttu-id="d249c-140">说明</span><span class="sxs-lookup"><span data-stu-id="d249c-140">Description</span></span>|
|:---------------|:--------|:--------|:--------|:----------|
|<span data-ttu-id="d249c-141">clientId</span><span class="sxs-lookup"><span data-stu-id="d249c-141">clientId</span></span>|<span data-ttu-id="d249c-142">字符串</span><span class="sxs-lookup"><span data-stu-id="d249c-142">String</span></span>|<span data-ttu-id="d249c-143">是</span><span class="sxs-lookup"><span data-stu-id="d249c-143">Yes</span></span>|<span data-ttu-id="d249c-144">否</span><span class="sxs-lookup"><span data-stu-id="d249c-144">No</span></span>|<span data-ttu-id="d249c-145">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="d249c-145">The client ID for the application.</span></span> <span data-ttu-id="d249c-146">这是注册的标识提供程序的应用程序时所获得的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="d249c-146">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="d249c-147">client_secret</span><span class="sxs-lookup"><span data-stu-id="d249c-147">clientSecret</span></span>|<span data-ttu-id="d249c-148">字符串</span><span class="sxs-lookup"><span data-stu-id="d249c-148">String</span></span>|<span data-ttu-id="d249c-149">是</span><span class="sxs-lookup"><span data-stu-id="d249c-149">Yes</span></span>|<span data-ttu-id="d249c-150">否</span><span class="sxs-lookup"><span data-stu-id="d249c-150">No</span></span>|<span data-ttu-id="d249c-151">应用程序客户端机密。</span><span class="sxs-lookup"><span data-stu-id="d249c-151">The client secret for the application.</span></span> <span data-ttu-id="d249c-152">这是注册的标识提供程序的应用程序时所获得的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="d249c-152">This is the client secret obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="d249c-153">这是只写。</span><span class="sxs-lookup"><span data-stu-id="d249c-153">This is write-only.</span></span> <span data-ttu-id="d249c-154">读取的操作将返回"\*\*\*\*"。</span><span class="sxs-lookup"><span data-stu-id="d249c-154">A read operation will return "\*\*\*\*".</span></span>|
|<span data-ttu-id="d249c-155">id</span><span class="sxs-lookup"><span data-stu-id="d249c-155">id</span></span>|<span data-ttu-id="d249c-156">字符串</span><span class="sxs-lookup"><span data-stu-id="d249c-156">String</span></span>|<span data-ttu-id="d249c-157">否</span><span class="sxs-lookup"><span data-stu-id="d249c-157">No</span></span>|<span data-ttu-id="d249c-158">否</span><span class="sxs-lookup"><span data-stu-id="d249c-158">No</span></span>|<span data-ttu-id="d249c-159">标识提供程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="d249c-159">The ID of the identity provider.</span></span>|
|<span data-ttu-id="d249c-160">name</span><span class="sxs-lookup"><span data-stu-id="d249c-160">name</span></span>|<span data-ttu-id="d249c-161">String</span><span class="sxs-lookup"><span data-stu-id="d249c-161">String</span></span>|<span data-ttu-id="d249c-162">否</span><span class="sxs-lookup"><span data-stu-id="d249c-162">No</span></span>|<span data-ttu-id="d249c-163">否</span><span class="sxs-lookup"><span data-stu-id="d249c-163">No</span></span>|<span data-ttu-id="d249c-164">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d249c-164">The display name of the identity provider.</span></span>|
|<span data-ttu-id="d249c-165">type</span><span class="sxs-lookup"><span data-stu-id="d249c-165">type</span></span>|<span data-ttu-id="d249c-166">String</span><span class="sxs-lookup"><span data-stu-id="d249c-166">String</span></span>|<span data-ttu-id="d249c-167">是</span><span class="sxs-lookup"><span data-stu-id="d249c-167">Yes</span></span>|<span data-ttu-id="d249c-168">否</span><span class="sxs-lookup"><span data-stu-id="d249c-168">No</span></span>|<span data-ttu-id="d249c-169">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="d249c-169">The identity provider type.</span></span> <span data-ttu-id="d249c-170">它必须是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="d249c-170">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="d249c-171">Microsoft</span><span class="sxs-lookup"><span data-stu-id="d249c-171">Microsoft</span></span><li/><span data-ttu-id="d249c-172">Google</span><span class="sxs-lookup"><span data-stu-id="d249c-172">Google</span></span><li/><span data-ttu-id="d249c-173">Amazon</span><span class="sxs-lookup"><span data-stu-id="d249c-173">Amazon</span></span><li/><span data-ttu-id="d249c-174">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="d249c-174">LinkedIn</span></span><li/><span data-ttu-id="d249c-175">Facebook</span><span class="sxs-lookup"><span data-stu-id="d249c-175">Facebook</span></span></ul>|

### <a name="where-to-get-the-client-id-and-secret"></a><span data-ttu-id="d249c-176">了解客户端 ID 和机密</span><span class="sxs-lookup"><span data-stu-id="d249c-176">Where to get the client ID and secret</span></span>

<span data-ttu-id="d249c-177">每个身份提供程序已创建应用程序注册的过程。</span><span class="sxs-lookup"><span data-stu-id="d249c-177">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="d249c-178">例如，用户创建应用程序注册与 Facebook 在[developers.facebook.com](https://developers.facebook.com/)。</span><span class="sxs-lookup"><span data-stu-id="d249c-178">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="d249c-179">生成客户端 ID 和客户端机密可以传递给[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。</span><span class="sxs-lookup"><span data-stu-id="d249c-179">The resulting client ID and client secret can be passed to [create identityProvider](../api/identityprovider-post-identityproviders.md).</span></span> <span data-ttu-id="d249c-180">然后，可以对任何身份验证的租户的身份提供程序联盟的目录中的每个用户对象。</span><span class="sxs-lookup"><span data-stu-id="d249c-180">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="d249c-181">这就使用户通过身份提供程序的登录页上输入凭据来登录。</span><span class="sxs-lookup"><span data-stu-id="d249c-181">This enables the user to sign in by entering credentials on the identity provider's sign in page.</span></span> <span data-ttu-id="d249c-182">按之前租户颁发一个令牌对应用程序的 Azure AD 验证身份提供程序中的令牌。</span><span class="sxs-lookup"><span data-stu-id="d249c-182">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d249c-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d249c-183">JSON representation</span></span>

<span data-ttu-id="d249c-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d249c-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
