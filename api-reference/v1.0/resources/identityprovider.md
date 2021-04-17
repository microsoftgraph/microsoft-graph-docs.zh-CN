---
title: identityProvider 资源类型
description: 表示 Azure Active Directory (Azure AD) 标识提供程序。
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c03d1a47925456038ebaf24b96d93e73d844f16c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882192"
---
# <a name="identityprovider-resource-type"></a><span data-ttu-id="b6e5f-103">identityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6e5f-103">identityProvider resource type</span></span>

<span data-ttu-id="b6e5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6e5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6e5f-105">表示 Azure Active Directory (Azure AD) 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-105">Represents an Azure Active Directory (Azure AD) identity provider.</span></span> <span data-ttu-id="b6e5f-106">标识提供者 **Microsoft**、 **Google**、 **Facebook**、 **Amazon**、  **LinkedIn** 或 **Twitter**。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-106">The identity provider can be **Microsoft**, **Google**, **Facebook**, **Amazon**,  **LinkedIn**, or **Twitter**.</span></span> <span data-ttu-id="b6e5f-107">以下标识提供者为预览版： **微博**、 **QQ**、 **微信**、 **GitHub** 以及任何 OpenID Connect 支持的提供商。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-107">The following Identity Providers are in Preview: **Weibo**, **QQ**, **WeChat**, **GitHub** and any OpenID Connect supported providers.</span></span> 

<span data-ttu-id="b6e5f-108">通过在 Azure AD B2C 中配置标识提供程序，使用户能够执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b6e5f-108">Configuring an identity provider in your Azure AD B2C tenant enables users to:</span></span>

* <span data-ttu-id="b6e5f-109">在使用者应用程序中通过社交帐户进行注册和登录。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-109">Sign up and sign in using a social account in a consumer application.</span></span> <span data-ttu-id="b6e5f-110">例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户注册服务。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-110">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account.</span></span>
* <span data-ttu-id="b6e5f-111">将现有本地帐户链接到使用者应用程序中的社交帐户。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-111">Link an existing local account to a social account in a consumer application.</span></span> <span data-ttu-id="b6e5f-112">例如，用户已在应用程序中创建用户名和密码（本地帐户）。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-112">For example, a user has created a username and password (local account) in the application.</span></span> <span data-ttu-id="b6e5f-113">之后，用户决定将现有本地帐户链接到其 Facebook 帐户，以便能使用 Facebook 进行登录。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-113">The user later decides to link the existing local account to their Facebook account so they can sign in using Facebook.</span></span>

<span data-ttu-id="b6e5f-114">通过在 Azure AD B2C 中配置标识提供程序，可实现之后的 B2B 来宾方案。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-114">Configuring an identity provider in your Azure AD tenant enables future B2B guest scenarios.</span></span> <span data-ttu-id="b6e5f-115">例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-115">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="b6e5f-116">Gmail 将使用其 Google 帐户凭据来验证和访问文档。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-116">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

## <a name="methods"></a><span data-ttu-id="b6e5f-117">方法</span><span class="sxs-lookup"><span data-stu-id="b6e5f-117">Methods</span></span>

| <span data-ttu-id="b6e5f-118">方法</span><span class="sxs-lookup"><span data-stu-id="b6e5f-118">Method</span></span>       | <span data-ttu-id="b6e5f-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6e5f-119">Return Type</span></span>  |<span data-ttu-id="b6e5f-120">说明</span><span class="sxs-lookup"><span data-stu-id="b6e5f-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6e5f-121">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-121">Get identityProvider</span></span>](../api/identityprovider-get.md) |<span data-ttu-id="b6e5f-122">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-122">identityProvider</span></span>|<span data-ttu-id="b6e5f-123">读取现有 identityProvider 中的属性。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-123">Read properties of an existing identityProvider.</span></span>|
|[<span data-ttu-id="b6e5f-124">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-124">Create identityProvider</span></span>](../api/identityprovider-post-identityproviders.md)|<span data-ttu-id="b6e5f-125">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-125">identityProvider</span></span>|<span data-ttu-id="b6e5f-126">新建 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-126">Create a new identityProvider.</span></span>|
|[<span data-ttu-id="b6e5f-127">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-127">Update identityProvider</span></span>](../api/identityprovider-update.md)|<span data-ttu-id="b6e5f-128">无</span><span class="sxs-lookup"><span data-stu-id="b6e5f-128">None</span></span>|<span data-ttu-id="b6e5f-129">更新现有的 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-129">Update an existing identityProvider.</span></span>|
|[<span data-ttu-id="b6e5f-130">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-130">Delete identityProvider</span></span>](../api/identityprovider-delete.md)|<span data-ttu-id="b6e5f-131">无</span><span class="sxs-lookup"><span data-stu-id="b6e5f-131">None</span></span>|<span data-ttu-id="b6e5f-132">删除现有的 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-132">Delete an existing identityProvider.</span></span>|
|[<span data-ttu-id="b6e5f-133">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6e5f-133">List identityProviders</span></span>](../api/identityprovider-list.md)|<span data-ttu-id="b6e5f-134">identityProvider 集合</span><span class="sxs-lookup"><span data-stu-id="b6e5f-134">identityProvider collection</span></span>|<span data-ttu-id="b6e5f-135">列出在租户中配置的所有 identityProvider。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-135">List all identityProviders configured in a tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6e5f-136">属性</span><span class="sxs-lookup"><span data-stu-id="b6e5f-136">Properties</span></span>

|<span data-ttu-id="b6e5f-137">属性</span><span class="sxs-lookup"><span data-stu-id="b6e5f-137">Property</span></span>|<span data-ttu-id="b6e5f-138">类型</span><span class="sxs-lookup"><span data-stu-id="b6e5f-138">Type</span></span>|<span data-ttu-id="b6e5f-139">说明</span><span class="sxs-lookup"><span data-stu-id="b6e5f-139">Description</span></span>|
|:---------------|:--------|:--------|
|<span data-ttu-id="b6e5f-140">clientId</span><span class="sxs-lookup"><span data-stu-id="b6e5f-140">clientId</span></span>|<span data-ttu-id="b6e5f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b6e5f-141">String</span></span>|<span data-ttu-id="b6e5f-142">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-142">The client ID for the application.</span></span> <span data-ttu-id="b6e5f-143">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-143">This is the client ID obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="b6e5f-144">必填。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-144">Required.</span></span> <span data-ttu-id="b6e5f-145">不可为空。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-145">Not nullable.</span></span>|
|<span data-ttu-id="b6e5f-146">clientSecret</span><span class="sxs-lookup"><span data-stu-id="b6e5f-146">clientSecret</span></span>|<span data-ttu-id="b6e5f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="b6e5f-147">String</span></span>|<span data-ttu-id="b6e5f-148">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-148">The client secret for the application.</span></span> <span data-ttu-id="b6e5f-149">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-149">This is the client secret obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="b6e5f-150">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-150">This is write-only.</span></span> <span data-ttu-id="b6e5f-151">读取操作将返回“`****`”。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-151">A read operation will return `****`.</span></span>  <span data-ttu-id="b6e5f-152">必填。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-152">Required.</span></span> <span data-ttu-id="b6e5f-153">不可为空。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-153">Not nullable.</span></span>|
|<span data-ttu-id="b6e5f-154">id</span><span class="sxs-lookup"><span data-stu-id="b6e5f-154">id</span></span>|<span data-ttu-id="b6e5f-155">字符串</span><span class="sxs-lookup"><span data-stu-id="b6e5f-155">String</span></span>|<span data-ttu-id="b6e5f-156">标识提供程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-156">The ID of the identity provider.</span></span>|
|<span data-ttu-id="b6e5f-157">name</span><span class="sxs-lookup"><span data-stu-id="b6e5f-157">name</span></span>|<span data-ttu-id="b6e5f-158">字符串</span><span class="sxs-lookup"><span data-stu-id="b6e5f-158">String</span></span>|<span data-ttu-id="b6e5f-159">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-159">The display name of the identity provider.</span></span> <span data-ttu-id="b6e5f-160">不可为空。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-160">Not nullable.</span></span>|
|<span data-ttu-id="b6e5f-161">type</span><span class="sxs-lookup"><span data-stu-id="b6e5f-161">type</span></span>|<span data-ttu-id="b6e5f-162">字符串</span><span class="sxs-lookup"><span data-stu-id="b6e5f-162">String</span></span>|<span data-ttu-id="b6e5f-163">身份提供程序类型是必填字段。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-163">The identity provider type is a required field.</span></span> <span data-ttu-id="b6e5f-164">对于 B2B 方案： `Google`， `Facebook`。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-164">For B2B scenario: `Google`, `Facebook`.</span></span> <span data-ttu-id="b6e5f-165">对于 B2C 方案： `Microsoft`、 `Google`、 `Amazon`、 `LinkedIn`、 `Facebook`、 `GitHub`、 `Twitter`、 `Weibo`、`QQ`、 `WeChat`、 `OpenIDConnect`。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-165">For B2C scenario: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`, `OpenIDConnect`.</span></span> <span data-ttu-id="b6e5f-166">不可为空。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-166">Not nullable.</span></span>|

### <a name="where-to-get-the-client-id-and-secret"></a><span data-ttu-id="b6e5f-167">获取客户端 ID 和密码的位置</span><span class="sxs-lookup"><span data-stu-id="b6e5f-167">Where to get the client ID and secret</span></span>

<span data-ttu-id="b6e5f-168">每个标识提供程序都有一个用于创建应用注册的进程。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-168">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="b6e5f-169">例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-169">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="b6e5f-170">生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-170">The resulting client ID and client secret can be passed to [create identityProvider](../api/identityprovider-post-identityproviders.md).</span></span> <span data-ttu-id="b6e5f-171">然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-171">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="b6e5f-172">这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-172">This enables the user to sign in by entering credentials on the identity provider's sign in page.</span></span> <span data-ttu-id="b6e5f-173">来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-173">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6e5f-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6e5f-174">JSON representation</span></span>

<span data-ttu-id="b6e5f-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6e5f-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProvider"
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

