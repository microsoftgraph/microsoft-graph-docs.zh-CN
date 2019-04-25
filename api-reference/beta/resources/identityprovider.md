---
title: identityProvider 资源类型
description: 表示 Azure Active Directory (Azure AD) 标识提供程序。 标识提供程序可以是 Microsoft、Google、Facebook、Amazon 或 LinkedIn。
localization_priority: Normal
ms.openlocfilehash: afd21635d932582f2a9ee6c2cde1cf45a9d4260f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547261"
---
# <a name="identityprovider-resource-type"></a><span data-ttu-id="db5c8-104">identityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="db5c8-104">identityProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db5c8-105">表示 Azure Active Directory (Azure AD) 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="db5c8-105">Represents an Azure Active Directory (Azure AD) identity provider.</span></span> <span data-ttu-id="db5c8-106">标识提供程序可以是 Microsoft、Google、Facebook、Amazon 或 LinkedIn。</span><span class="sxs-lookup"><span data-stu-id="db5c8-106">The identity provider can be Microsoft, Google, Facebook, Amazon, or LinkedIn.</span></span>

<span data-ttu-id="db5c8-107">在 Azure AD B2C 租户中配置标识提供程序可实现以下功能:</span><span class="sxs-lookup"><span data-stu-id="db5c8-107">Configuring an identity provider in your Azure AD B2C tenant enables:</span></span>

* <span data-ttu-id="db5c8-108">用户使用使用者应用程序中的社交帐户进行注册并登录。</span><span class="sxs-lookup"><span data-stu-id="db5c8-108">Users to sign up and sign in using a social account in a consumer application.</span></span> <span data-ttu-id="db5c8-109">例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户注册服务。</span><span class="sxs-lookup"><span data-stu-id="db5c8-109">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account.</span></span>
* <span data-ttu-id="db5c8-110">用户将现有本地帐户链接到使用者应用程序中的社交帐户。</span><span class="sxs-lookup"><span data-stu-id="db5c8-110">Users to link an existing local account to a social account in a consumer application.</span></span> <span data-ttu-id="db5c8-111">例如，用户已在应用程序中创建用户名和密码（本地帐户）。</span><span class="sxs-lookup"><span data-stu-id="db5c8-111">For example, a user has created a username and password (local account) in the application.</span></span> <span data-ttu-id="db5c8-112">之后，用户决定将现有本地帐户链接到其 Facebook 帐户，以便能使用 Facebook 进行登录。</span><span class="sxs-lookup"><span data-stu-id="db5c8-112">The user later decides to link the existing local account to their Facebook account so they can sign in using Facebook.</span></span>

<span data-ttu-id="db5c8-113">通过在 Azure AD B2C 中配置标识提供程序，可实现之后的 B2B 来宾方案。</span><span class="sxs-lookup"><span data-stu-id="db5c8-113">Configuring an identity provider in your Azure AD tenant enables future B2B guest scenarios.</span></span> <span data-ttu-id="db5c8-114">例如，某组织在 Office 365 中具有需要与 Gmail 用户共享的资源。</span><span class="sxs-lookup"><span data-stu-id="db5c8-114">For example, an organization has resources in Office 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="db5c8-115">Gmail 将使用其 Google 帐户凭据来验证和访问文档。</span><span class="sxs-lookup"><span data-stu-id="db5c8-115">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

## <a name="methods"></a><span data-ttu-id="db5c8-116">方法</span><span class="sxs-lookup"><span data-stu-id="db5c8-116">Methods</span></span>

| <span data-ttu-id="db5c8-117">方法</span><span class="sxs-lookup"><span data-stu-id="db5c8-117">Method</span></span>       | <span data-ttu-id="db5c8-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="db5c8-118">Return Type</span></span>  |<span data-ttu-id="db5c8-119">说明</span><span class="sxs-lookup"><span data-stu-id="db5c8-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db5c8-120">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-120">Get identityProvider</span></span>](../api/identityprovider-get.md) |<span data-ttu-id="db5c8-121">identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-121">identityProvider</span></span>|<span data-ttu-id="db5c8-122">读取现有 identityProvider 中的属性。</span><span class="sxs-lookup"><span data-stu-id="db5c8-122">Read properties of an existing identityProvider.</span></span>|
|[<span data-ttu-id="db5c8-123">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-123">Create identityProvider</span></span>](../api/identityprovider-post-identityproviders.md)|<span data-ttu-id="db5c8-124">identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-124">identityProvider</span></span>|<span data-ttu-id="db5c8-125">新建 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="db5c8-125">Create a new identityProvider.</span></span>|
|[<span data-ttu-id="db5c8-126">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-126">Update identityProvider</span></span>](../api/identityprovider-update.md)|<span data-ttu-id="db5c8-127">无</span><span class="sxs-lookup"><span data-stu-id="db5c8-127">None</span></span>|<span data-ttu-id="db5c8-128">更新现有的 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="db5c8-128">Update an existing identityProvider.</span></span>|
|[<span data-ttu-id="db5c8-129">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-129">Delete identityProvider</span></span>](../api/identityprovider-delete.md)|<span data-ttu-id="db5c8-130">无</span><span class="sxs-lookup"><span data-stu-id="db5c8-130">None</span></span>|<span data-ttu-id="db5c8-131">删除现有的 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="db5c8-131">Delete an existing identityProvider.</span></span>|
|[<span data-ttu-id="db5c8-132">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="db5c8-132">List identityProviders</span></span>](../api/identityprovider-list.md)|<span data-ttu-id="db5c8-133">identityProvider 集合</span><span class="sxs-lookup"><span data-stu-id="db5c8-133">identityProvider collection</span></span>|<span data-ttu-id="db5c8-134">列出在租户中配置的所有 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="db5c8-134">List all identityProviders configured in a tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="db5c8-135">属性</span><span class="sxs-lookup"><span data-stu-id="db5c8-135">Properties</span></span>

|<span data-ttu-id="db5c8-136">属性</span><span class="sxs-lookup"><span data-stu-id="db5c8-136">Property</span></span>|<span data-ttu-id="db5c8-137">类型</span><span class="sxs-lookup"><span data-stu-id="db5c8-137">Type</span></span>|<span data-ttu-id="db5c8-138">必需</span><span class="sxs-lookup"><span data-stu-id="db5c8-138">Required</span></span>|<span data-ttu-id="db5c8-139">可为空</span><span class="sxs-lookup"><span data-stu-id="db5c8-139">Nullable</span></span>|<span data-ttu-id="db5c8-140">说明</span><span class="sxs-lookup"><span data-stu-id="db5c8-140">Description</span></span>|
|:---------------|:--------|:--------|:--------|:----------|
|<span data-ttu-id="db5c8-141">clientId</span><span class="sxs-lookup"><span data-stu-id="db5c8-141">clientId</span></span>|<span data-ttu-id="db5c8-142">字符串</span><span class="sxs-lookup"><span data-stu-id="db5c8-142">String</span></span>|<span data-ttu-id="db5c8-143">是</span><span class="sxs-lookup"><span data-stu-id="db5c8-143">Yes</span></span>|<span data-ttu-id="db5c8-144">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-144">No</span></span>|<span data-ttu-id="db5c8-145">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="db5c8-145">The client ID for the application.</span></span> <span data-ttu-id="db5c8-146">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="db5c8-146">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="db5c8-147">clientSecret</span><span class="sxs-lookup"><span data-stu-id="db5c8-147">clientSecret</span></span>|<span data-ttu-id="db5c8-148">字符串</span><span class="sxs-lookup"><span data-stu-id="db5c8-148">String</span></span>|<span data-ttu-id="db5c8-149">是</span><span class="sxs-lookup"><span data-stu-id="db5c8-149">Yes</span></span>|<span data-ttu-id="db5c8-150">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-150">No</span></span>|<span data-ttu-id="db5c8-151">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="db5c8-151">The client secret for the application.</span></span> <span data-ttu-id="db5c8-152">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="db5c8-152">This is the client secret obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="db5c8-153">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="db5c8-153">This is write-only.</span></span> <span data-ttu-id="db5c8-154">读取操作将返回“\*\*\*\*”。</span><span class="sxs-lookup"><span data-stu-id="db5c8-154">A read operation will return "\*\*\*\*".</span></span>|
|<span data-ttu-id="db5c8-155">id</span><span class="sxs-lookup"><span data-stu-id="db5c8-155">id</span></span>|<span data-ttu-id="db5c8-156">字符串</span><span class="sxs-lookup"><span data-stu-id="db5c8-156">String</span></span>|<span data-ttu-id="db5c8-157">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-157">No</span></span>|<span data-ttu-id="db5c8-158">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-158">No</span></span>|<span data-ttu-id="db5c8-159">标识提供程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="db5c8-159">The ID of the identity provider.</span></span>|
|<span data-ttu-id="db5c8-160">name</span><span class="sxs-lookup"><span data-stu-id="db5c8-160">name</span></span>|<span data-ttu-id="db5c8-161">String</span><span class="sxs-lookup"><span data-stu-id="db5c8-161">String</span></span>|<span data-ttu-id="db5c8-162">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-162">No</span></span>|<span data-ttu-id="db5c8-163">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-163">No</span></span>|<span data-ttu-id="db5c8-164">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="db5c8-164">The display name of the identity provider.</span></span>|
|<span data-ttu-id="db5c8-165">type</span><span class="sxs-lookup"><span data-stu-id="db5c8-165">type</span></span>|<span data-ttu-id="db5c8-166">字符串</span><span class="sxs-lookup"><span data-stu-id="db5c8-166">String</span></span>|<span data-ttu-id="db5c8-167">是</span><span class="sxs-lookup"><span data-stu-id="db5c8-167">Yes</span></span>|<span data-ttu-id="db5c8-168">否</span><span class="sxs-lookup"><span data-stu-id="db5c8-168">No</span></span>|<span data-ttu-id="db5c8-169">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="db5c8-169">The identity provider type.</span></span> <span data-ttu-id="db5c8-170">它必须是下列值之一:</span><span class="sxs-lookup"><span data-stu-id="db5c8-170">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="db5c8-171">Microsoft</span><span class="sxs-lookup"><span data-stu-id="db5c8-171">Microsoft</span></span><li/><span data-ttu-id="db5c8-172">Google</span><span class="sxs-lookup"><span data-stu-id="db5c8-172">Google</span></span><li/><span data-ttu-id="db5c8-173">Amazon</span><span class="sxs-lookup"><span data-stu-id="db5c8-173">Amazon</span></span><li/><span data-ttu-id="db5c8-174">领英</span><span class="sxs-lookup"><span data-stu-id="db5c8-174">LinkedIn</span></span><li/><span data-ttu-id="db5c8-175">Facebook</span><span class="sxs-lookup"><span data-stu-id="db5c8-175">Facebook</span></span></ul>|

### <a name="where-to-get-the-client-id-and-secret"></a><span data-ttu-id="db5c8-176">获取客户端 ID 和密码的位置</span><span class="sxs-lookup"><span data-stu-id="db5c8-176">Where to get the client ID and secret</span></span>

<span data-ttu-id="db5c8-177">每个标识提供程序都有一个用于创建应用注册的进程。</span><span class="sxs-lookup"><span data-stu-id="db5c8-177">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="db5c8-178">例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。</span><span class="sxs-lookup"><span data-stu-id="db5c8-178">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="db5c8-179">生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。</span><span class="sxs-lookup"><span data-stu-id="db5c8-179">The resulting client ID and client secret can be passed to [create identityProvider](../api/identityprovider-post-identityproviders.md).</span></span> <span data-ttu-id="db5c8-180">然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="db5c8-180">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="db5c8-181">这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。</span><span class="sxs-lookup"><span data-stu-id="db5c8-181">This enables the user to sign in by entering credentials on the identity provider's sign in page.</span></span> <span data-ttu-id="db5c8-182">来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。</span><span class="sxs-lookup"><span data-stu-id="db5c8-182">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db5c8-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db5c8-183">JSON representation</span></span>

<span data-ttu-id="db5c8-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db5c8-184">The following is a JSON representation of the resource.</span></span>

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
