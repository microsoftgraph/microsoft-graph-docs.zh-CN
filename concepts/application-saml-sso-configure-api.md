---
title: 使用 Microsoft Graph API 配置基于 SAML 的单一登录
description: 了解如何通过使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录来节省时间。
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: 095ce00cafcc07c17de5e93b766fb5d12def4723
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373569"
---
# <a name="automate-saml-based-sso-app-configuration-with-microsoft-graph-api"></a><span data-ttu-id="cd30c-103">使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置</span><span class="sxs-lookup"><span data-stu-id="cd30c-103">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>

<span data-ttu-id="cd30c-104">在本文中，您将学习如何从 Azure Active Directory（Azure AD）库中创建和配置应用程序。</span><span class="sxs-lookup"><span data-stu-id="cd30c-104">In this article, you'll learn how to create and configure an application from the Azure Active Directory (Azure AD) Gallery.</span></span> <span data-ttu-id="cd30c-105">本文使用 AWS 作为示例，但可以针对 Azure AD 库中的任何基于 SAML 的应用使用本文中的步骤。</span><span class="sxs-lookup"><span data-stu-id="cd30c-105">This article uses AWS as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

<span data-ttu-id="cd30c-106">**使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录的步骤**</span><span class="sxs-lookup"><span data-stu-id="cd30c-106">**Steps to use Microsoft Graph APIs to automate configuration of SAML-based single sign-on**</span></span>

| <span data-ttu-id="cd30c-107">步骤</span><span class="sxs-lookup"><span data-stu-id="cd30c-107">Step</span></span>  | <span data-ttu-id="cd30c-108">详细信息</span><span class="sxs-lookup"><span data-stu-id="cd30c-108">Details</span></span>  |
|---------|---------|
| [<span data-ttu-id="cd30c-109">1. 创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="cd30c-109">1. Create the gallery application</span></span>](#step-1-create-the-gallery-application) | <span data-ttu-id="cd30c-110">登录到 API 客户端</span><span class="sxs-lookup"><span data-stu-id="cd30c-110">Sign in to the API client</span></span> <br> <span data-ttu-id="cd30c-111">检索库应用</span><span class="sxs-lookup"><span data-stu-id="cd30c-111">Retrieve the gallery application</span></span> <br> <span data-ttu-id="cd30c-112">创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="cd30c-112">Create the gallery application</span></span>|
| [<span data-ttu-id="cd30c-113">2. 配置单一登录</span><span class="sxs-lookup"><span data-stu-id="cd30c-113">2. Configure single sign-on</span></span>](#step-2-configure-single-sign-on) | <span data-ttu-id="cd30c-114">检索应用对象 ID 和服务主体对象 ID</span><span class="sxs-lookup"><span data-stu-id="cd30c-114">Retrieve app object ID and service principal object ID</span></span> <br> <span data-ttu-id="cd30c-115">设置单一登录模式</span><span class="sxs-lookup"><span data-stu-id="cd30c-115">Set single sign-on mode</span></span> <br> <span data-ttu-id="cd30c-116">设置基本 SAML URL、例如标识符、回复 URL、登录 URL</span><span class="sxs-lookup"><span data-stu-id="cd30c-116">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span> <br> <span data-ttu-id="cd30c-117">添加应用程序角色（可选）</span><span class="sxs-lookup"><span data-stu-id="cd30c-117">Add app roles (Optional)</span></span>|
| [<span data-ttu-id="cd30c-118">3. 配置声明映射</span><span class="sxs-lookup"><span data-stu-id="cd30c-118">3. Configure claims mapping</span></span>](#step-3-configure-claims-mapping) | <span data-ttu-id="cd30c-119">创建声明映射策略</span><span class="sxs-lookup"><span data-stu-id="cd30c-119">Create claims mapping policy</span></span> <br> <span data-ttu-id="cd30c-120">向服务主体分配声明映射策略</span><span class="sxs-lookup"><span data-stu-id="cd30c-120">Assign claims mapping policy to service principal</span></span>|
| [<span data-ttu-id="cd30c-121">4. 配置签名证书</span><span class="sxs-lookup"><span data-stu-id="cd30c-121">4. Configure signing certificate</span></span>](#step-4-configure-signing-certificate) | <span data-ttu-id="cd30c-122">创建证书</span><span class="sxs-lookup"><span data-stu-id="cd30c-122">Create a certificate</span></span> <BR> <span data-ttu-id="cd30c-123">添加自定义签名密钥</span><span class="sxs-lookup"><span data-stu-id="cd30c-123">Add a custom signing key</span></span> <br> <span data-ttu-id="cd30c-124">激活自定义签名密钥</span><span class="sxs-lookup"><span data-stu-id="cd30c-124">Activate the custom signing key</span></span>|
| [<span data-ttu-id="cd30c-125">5. 分配用户</span><span class="sxs-lookup"><span data-stu-id="cd30c-125">5. Assign users</span></span>](#step-5-assign-users) | <span data-ttu-id="cd30c-126">向应用程序分配用户和组</span><span class="sxs-lookup"><span data-stu-id="cd30c-126">Assign users and groups to the application</span></span>
| [<span data-ttu-id="cd30c-127">6. 配置应用程序端</span><span class="sxs-lookup"><span data-stu-id="cd30c-127">6. Configure the application side</span></span>](#step-6-configure-the-application-side)| <span data-ttu-id="cd30c-128">获取 Azure AD SAML 元数据</span><span class="sxs-lookup"><span data-stu-id="cd30c-128">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="cd30c-129">**文章中使用的所有 API 列表**</span><span class="sxs-lookup"><span data-stu-id="cd30c-129">**List of all APIs used in the article**</span></span>

<span data-ttu-id="cd30c-130">请确保你具有相应的权限来调用以下 API。</span><span class="sxs-lookup"><span data-stu-id="cd30c-130">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="cd30c-131">资源类型</span><span class="sxs-lookup"><span data-stu-id="cd30c-131">Resource type</span></span> |<span data-ttu-id="cd30c-132">方法</span><span class="sxs-lookup"><span data-stu-id="cd30c-132">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="cd30c-133">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd30c-133">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-beta)|[<span data-ttu-id="cd30c-134">列出 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd30c-134">List applicationTemplate</span></span>](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) <br>[<span data-ttu-id="cd30c-135">实例化 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd30c-135">Instantiate applicationTemplate</span></span>](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta)|
|[<span data-ttu-id="cd30c-136">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="cd30c-136">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="cd30c-137">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="cd30c-137">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="cd30c-138">创建 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="cd30c-138">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="cd30c-139">分配 claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="cd30c-139">Assign claimsMappingPolicies</span></span>](/graph/api/serviceprincipal-post-claimsmappingpolicies?tabs=http&view=graph-rest-beta)|
|[<span data-ttu-id="cd30c-140">applications</span><span class="sxs-lookup"><span data-stu-id="cd30c-140">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)|[<span data-ttu-id="cd30c-141">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="cd30c-141">Update application</span></span>](/graph/api/application-update?tabs=http&view=graph-rest-1.0)|
|[<span data-ttu-id="cd30c-142">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="cd30c-142">claimsMappingPolicy</span></span>](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)| [<span data-ttu-id="cd30c-143">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="cd30c-143">Create claimsMappingPolicy</span></span>](/graph/api/claimsmappingpolicy-post-claimsmappingpolicies?tabs=http&view=graph-rest-beta)

>[!NOTE]
><span data-ttu-id="cd30c-144">本文中所示的响应对象可能会被缩短以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="cd30c-144">The response objects shown in this article might be shortened for readability.</span></span> <span data-ttu-id="cd30c-145">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cd30c-145">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="cd30c-146">第 1 步：创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="cd30c-146">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="cd30c-147">登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端</span><span class="sxs-lookup"><span data-stu-id="cd30c-147">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="cd30c-148">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-148">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="cd30c-149">选择**使用 Microsoft 登录**，然后使用 Azure AD 全局管理员或 App Admin 凭据登录。</span><span class="sxs-lookup"><span data-stu-id="cd30c-149">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="cd30c-150">成功登录后，将在左侧窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="cd30c-150">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="cd30c-151">检索库应用程序模板标识符</span><span class="sxs-lookup"><span data-stu-id="cd30c-151">Retrieve the gallery application template identifier</span></span>

<span data-ttu-id="cd30c-152">Azure AD 应用程序库中的每个应用程序都有一个[应用程序模板](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta)，用于描述该应用程序的元数据。</span><span class="sxs-lookup"><span data-stu-id="cd30c-152">Applications in the Azure AD application gallery each have an [application template](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) that describes the metadata for that application.</span></span> <span data-ttu-id="cd30c-153">使用此模板，可以在租户中创建应用程序和服务主体的实例以进行管理。</span><span class="sxs-lookup"><span data-stu-id="cd30c-153">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="cd30c-154">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd30c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd30c-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="cd30c-156">C#</span><span class="sxs-lookup"><span data-stu-id="cd30c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd30c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd30c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd30c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd30c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd30c-159">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
    "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "Amazon Web Services (AWS)",
        "homePageUrl": "http://aws.amazon.com/",
        "supportedSingleSignOnModes": [
             "password",
             "saml",
             "external"
         ],
         "supportedProvisioningTypes": [
             "sync"
         ],
         "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
         "categories": [
             "developerServices"
         ],
         "publisher": "Amazon",
         "description": null    
  
}
```

### <a name="create-the-gallery-application"></a><span data-ttu-id="cd30c-160">创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="cd30c-160">Create the gallery application</span></span>

<span data-ttu-id="cd30c-161">使用在上一步中为应用程序检索的模板ID，在租户中为应用和服务主题[创建实例](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-161">Using the template ID that you retrieved for your application in the last step, [create an instance](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) of the application and service principal in your tenant.</span></span>

> [!NOTE] 
> <span data-ttu-id="cd30c-162">可以使用 applicationTemplate API 实例化[非库应用程序](/azure/active-directory/manage-apps/view-applications-portal)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-162">You can use applicationTemplate API to instantiate [Non-Gallery apps](/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="cd30c-163">使用 applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`。</span><span class="sxs-lookup"><span data-stu-id="cd30c-163">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

> [!NOTE]
> <span data-ttu-id="cd30c-164">留出一些时间将应用程序配置到 Azure AD 租户中。</span><span class="sxs-lookup"><span data-stu-id="cd30c-164">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="cd30c-165">这不是即时的。</span><span class="sxs-lookup"><span data-stu-id="cd30c-165">It is not instant.</span></span> <span data-ttu-id="cd30c-166">一种策略是每 5-10秒 对应用程序/服务主体对象执行 GET 查询，直到查询成功。</span><span class="sxs-lookup"><span data-stu-id="cd30c-166">One strategy is to do a GET query on the application / service principal object every 5-10 seconds until the query is successful.</span></span>


#### <a name="request"></a><span data-ttu-id="cd30c-167">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-167">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd30c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd30c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```
# <a name="c"></a>[<span data-ttu-id="cd30c-169">C#</span><span class="sxs-lookup"><span data-stu-id="cd30c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd30c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd30c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd30c-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd30c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd30c-172">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-172">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json


{
    "application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63",
        "appId": "92653dd4-aa3a-3323-80cf-e8cfefcc8d5d",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "AWS Contoso",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "logoutUrl": null,
        "samlMetadataUrl": null,
    },
    "servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e",
        "appDisplayName": "AWS Contoso",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "appRoleAssignmentRequired": true,
        "displayName": "My custom name",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "servicePrincipalNames": [
            "93653dd4-aa3a-4323-80cf-e8cfefcc8d7d"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
    }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="cd30c-173">第 2 步：配置单一登录</span><span class="sxs-lookup"><span data-stu-id="cd30c-173">Step 2: Configure single sign-on</span></span>

### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="cd30c-174">检索应用对象 ID 和服务主体对象 ID</span><span class="sxs-lookup"><span data-stu-id="cd30c-174">Retrieve app object ID and service principal object ID</span></span>

<span data-ttu-id="cd30c-175">使用上一次调用的响应检索并保存应用程序对象 ID 和服务主体对象 ID。</span><span class="sxs-lookup"><span data-stu-id="cd30c-175">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>

```
"application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63"
}
"servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
### <a name="set-single-sign-on-mode"></a><span data-ttu-id="cd30c-176">设置单一登录模式</span><span class="sxs-lookup"><span data-stu-id="cd30c-176">Set single sign-on mode</span></span>

<span data-ttu-id="cd30c-177">在此示例中，将在 [ servicePrincipal 资源类型](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)中将 `saml` 设置为单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="cd30c-177">In this example, you'll set `saml` as the single sign-on mode in the [servicePrincipal resource type](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).</span></span> <span data-ttu-id="cd30c-178">可以配置的其他 SAML SSO 属性是：`notificationEmailAddresses`、`loginUrl`、和 `samlSingleSignOnSettings.relayState`。</span><span class="sxs-lookup"><span data-stu-id="cd30c-178">Other SAML SSO properties that you can configure are: `notificationEmailAddresses`, `loginUrl`, and `samlSingleSignOnSettings.relayState`.</span></span>

<span data-ttu-id="cd30c-179">在此查询生效之前，需要在 Graph Explorer 中的**修改权限**选项卡上表示同意。</span><span class="sxs-lookup"><span data-stu-id="cd30c-179">Before this query will work you need to provide consent on the **Modify permissions** tab in Graph Explorer.</span></span> <span data-ttu-id="cd30c-180">另外，请确保你使用的是先前获得的 **servicePrincipal** ID。</span><span class="sxs-lookup"><span data-stu-id="cd30c-180">Also, make sure you are using the **servicePrincipal** ID that you obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="cd30c-181">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-181">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd30c-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd30c-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: servicePrincipal/json

{
    "preferredSingleSignOnMode": "saml"
}
```
# <a name="c"></a>[<span data-ttu-id="cd30c-183">C#</span><span class="sxs-lookup"><span data-stu-id="cd30c-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd30c-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd30c-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd30c-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd30c-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd30c-186">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls-such-as-identifier-reply-url-sign-on-url"></a><span data-ttu-id="cd30c-187">设置基本 SAML URL、例如标识符、回复 URL、登录 URL</span><span class="sxs-lookup"><span data-stu-id="cd30c-187">Set basic SAML URLs such as identifier, reply URL, sign-on URL</span></span>

<span data-ttu-id="cd30c-188">在应用程序对象中设置 AWS 的标识符并回复 URL。</span><span class="sxs-lookup"><span data-stu-id="cd30c-188">Set the identifier and reply URLs for AWS in the application object.</span></span>

<span data-ttu-id="cd30c-189">请确保你使用的是之前获取的 **application** id。</span><span class="sxs-lookup"><span data-stu-id="cd30c-189">Make sure you are using the **application** id obtained earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="cd30c-190">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd30c-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd30c-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/cbc071a6-0fa5-4859-8g55-e983ef63df63
Content-type: applications/json

{
    "web": {
        "redirectUris": [
            "https://signin.aws.amazon.com/saml"
        ] 
    },
    "identifierUris": [
        "https://signin.aws.amazon.com/saml"
    ]    
}
```
# <a name="c"></a>[<span data-ttu-id="cd30c-192">C#</span><span class="sxs-lookup"><span data-stu-id="cd30c-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd30c-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd30c-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd30c-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd30c-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd30c-195">Java</span><span class="sxs-lookup"><span data-stu-id="cd30c-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cd30c-196">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-196">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```
### <a name="add-app-roles-optional"></a><span data-ttu-id="cd30c-197">添加应用程序角色（可选）</span><span class="sxs-lookup"><span data-stu-id="cd30c-197">Add app roles (Optional)</span></span>

<span data-ttu-id="cd30c-198">如果应用程序需要令牌中的角色信息，请在应用程序对象中添加角色的定义。</span><span class="sxs-lookup"><span data-stu-id="cd30c-198">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> <span data-ttu-id="cd30c-199">对于 AWS，可以[启用用户配置](/azure/active-directory/app-provisioning/application-provisioning-configure-api)以从该 AWS 账户获取所有角色。</span><span class="sxs-lookup"><span data-stu-id="cd30c-199">For AWS, you can [enable user provisioning](/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> 

<span data-ttu-id="cd30c-200">有关详细信息，请参阅[配置 SAML 令牌中颁发的角色声明](/azure/active-directory/develop/active-directory-enterprise-app-role-management)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-200">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>

> [!NOTE] 
> <span data-ttu-id="cd30c-201">添加应用程序角色时，请勿修改默认应用程序角色 msiam_access。</span><span class="sxs-lookup"><span data-stu-id="cd30c-201">When adding app roles, don't modify the default app roles msiam_access.</span></span> 

#### <a name="request"></a><span data-ttu-id="cd30c-202">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-202">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd30c-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd30c-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: serviceprincipals/json

{
"appRoles": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "7dfd756e-8c27-4472-b2b7-38c17fc5de5e",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Admin,WAAD",
            "displayName": "Admin,WAAD",
            "id": "454dc4c2-8176-498e-99df-8c4efcde41ef",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Finance,WAAD",
            "displayName": "Finance,WAAD",
            "id": "8642d5fa-18a3-4245-ab8c-a96000c1a217",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
        }
    ]

}
```
# <a name="c"></a>[<span data-ttu-id="cd30c-204">C#</span><span class="sxs-lookup"><span data-stu-id="cd30c-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd30c-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd30c-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd30c-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd30c-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd30c-207">Java</span><span class="sxs-lookup"><span data-stu-id="cd30c-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd30c-208">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-208">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="cd30c-209">第 3 步：配置声明映射</span><span class="sxs-lookup"><span data-stu-id="cd30c-209">Step 3: Configure claims mapping</span></span>

### <a name="create-claims-mapping-policy"></a><span data-ttu-id="cd30c-210">创建声明映射策略</span><span class="sxs-lookup"><span data-stu-id="cd30c-210">Create claims mapping policy</span></span>

<span data-ttu-id="cd30c-211">除了基本声明之外，还为 Azure AD 配置以下声明以在 SAML 令牌中发出：</span><span class="sxs-lookup"><span data-stu-id="cd30c-211">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="cd30c-212">声明名称</span><span class="sxs-lookup"><span data-stu-id="cd30c-212">Claim name</span></span> | <span data-ttu-id="cd30c-213">源</span><span class="sxs-lookup"><span data-stu-id="cd30c-213">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="cd30c-214">assignedroles</span><span class="sxs-lookup"><span data-stu-id="cd30c-214">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="cd30c-215">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="cd30c-215">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="cd30c-216">"900"</span><span class="sxs-lookup"><span data-stu-id="cd30c-216">"900"</span></span> |
| <span data-ttu-id="cd30c-217">roles</span><span class="sxs-lookup"><span data-stu-id="cd30c-217">roles</span></span> | <span data-ttu-id="cd30c-218">assignedroles</span><span class="sxs-lookup"><span data-stu-id="cd30c-218">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="cd30c-219">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="cd30c-219">userprincipalname</span></span> |

<span data-ttu-id="cd30c-220">有关更多信息，请参阅[自定义令牌中发出的声明](/azure/active-directory/develop/active-directory-claims-mapping)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-220">For more information, see [Customize claims emitted in token](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>

> [!NOTE]
> <span data-ttu-id="cd30c-221">声明映射策略中的某些项区分大小写（例如“Version”）。</span><span class="sxs-lookup"><span data-stu-id="cd30c-221">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="cd30c-222">如果收到错误消息，例如“属性的值无效”，则可能是区分大小写的问题。</span><span class="sxs-lookup"><span data-stu-id="cd30c-222">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

#### <a name="request"></a><span data-ttu-id="cd30c-223">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-223">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd30c-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd30c-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```
# <a name="c"></a>[<span data-ttu-id="cd30c-225">C#</span><span class="sxs-lookup"><span data-stu-id="cd30c-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd30c-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd30c-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd30c-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd30c-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd30c-228">Java</span><span class="sxs-lookup"><span data-stu-id="cd30c-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd30c-229">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-229">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicies",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK
Content-type: claimsMappingPolicies/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "a7b19e62-9adb-4edb-8521-cd35305f095d",
    "deletedDateTime": null,
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-claims-mapping-policy-to-service-principal"></a><span data-ttu-id="cd30c-230">向服务主体分配声明映射策略</span><span class="sxs-lookup"><span data-stu-id="cd30c-230">Assign claims mapping policy to service principal</span></span>

#### <a name="request"></a><span data-ttu-id="cd30c-231">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-231">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/claimsMappingPolicies/$ref

Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/6b33aa8e-51f3-41a6-a0fd-d660d276197a"
}
```


#### <a name="response"></a><span data-ttu-id="cd30c-232">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-232">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-4-configure-signing-certificate"></a><span data-ttu-id="cd30c-233">第 4 步：配置签名证书</span><span class="sxs-lookup"><span data-stu-id="cd30c-233">Step 4: Configure signing certificate</span></span>

<span data-ttu-id="cd30c-234">默认情况下，使用 [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta) API 无法创建签名证书。</span><span class="sxs-lookup"><span data-stu-id="cd30c-234">Using the [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta) API doesn't create a signing certificate by default.</span></span> <span data-ttu-id="cd30c-235">创建自定义签名证书并将其分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="cd30c-235">Create your custom signing cert and assign it to the application.</span></span> 

### <a name="create-a-custom-signing-certificate"></a><span data-ttu-id="cd30c-236">创建自定义签名证书</span><span class="sxs-lookup"><span data-stu-id="cd30c-236">Create a custom signing certificate</span></span>

<span data-ttu-id="cd30c-237">要进行测试，可以使用以下 PowerShell 命令获取自签名证书。</span><span class="sxs-lookup"><span data-stu-id="cd30c-237">To test, you can use the following PowerShell command to get a self-signed certificate.</span></span> <span data-ttu-id="cd30c-238">然后需要使用其他工具手动操作和提取所需的值。</span><span class="sxs-lookup"><span data-stu-id="cd30c-238">You will then need to manipulate and pull the values you need manually using other tools.</span></span> <span data-ttu-id="cd30c-239">使用公司的最佳安全实践，创建用于生产的签名证书。</span><span class="sxs-lookup"><span data-stu-id="cd30c-239">Use the best security practice from your company to create a signing certificate for production.</span></span>

```powershell
Param(
    [Parameter(Mandatory=$true)]
    [string]$fqdn,
    [Parameter(Mandatory=$true)]
    [string]$pwd,
    [Parameter(Mandatory=$true)]
    [string]$location
) 

if (!$PSBoundParameters.ContainsKey('location'))
{
    $location = "."
} 

$cert = New-SelfSignedCertificate -certstorelocation cert:\currentuser\my -DnsName $fqdn
$pwdSecure = ConvertTo-SecureString -String $pwd -Force -AsPlainText
$path = 'cert:\currentuser\my\' + $cert.Thumbprint
$cerFile = $location + "\\" + $fqdn + ".cer"
$pfxFile = $location + "\\" + $fqdn + ".pfx" 

Export-PfxCertificate -cert $path -FilePath $pfxFile -Password $pwdSecure
Export-Certificate -cert $path -FilePath $cerFile
```

<span data-ttu-id="cd30c-240">或者，可以将以下 C# 控制台应用程序用作概念证明，以了解如何获取所需的值。</span><span class="sxs-lookup"><span data-stu-id="cd30c-240">Alternatively, the following C# console app can be used as a Proof of Concept to understand how the required values can be obtained.</span></span> <span data-ttu-id="cd30c-241">请注意，该代码仅用于**学习和参考**，不应在生产中直接使用。</span><span class="sxs-lookup"><span data-stu-id="cd30c-241">Note that this code is for **learning and reference ONLY** and should not be used as-is in production.</span></span>

```csharp
using System;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using System.Text;


/* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
 * This code uses a self signed certificate and should not be used 
 * in production. This code is for reference and learning ONLY.
 */
namespace Self_signed_cert
{
    class Program
    {
        static void Main(string[] args)
        {
            // Generate a guid to use as a password and then create the cert.
            string password = Guid.NewGuid().ToString();
            var selfsignedCert = buildSelfSignedServerCertificate(password);

            // Print values so we can copy paste into the JSON fields.
            // Print out the private key in base64 format.
            Console.WriteLine("Private Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Pfx, password)), Environment.NewLine);

            // Print out the start date in ISO 8601 format.
            DateTime startDate = DateTime.Parse(selfsignedCert.GetEffectiveDateString()).ToUniversalTime();
            Console.WriteLine("For All startDateTime: " + startDate.ToString("o"));

            // Print out the end date in ISO 8601 format.
            DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
            Console.WriteLine("For All endDateTime: " + endDate.ToString("o"));

            // Print the GUID used for keyId
            string signAndPasswordGuid = Guid.NewGuid().ToString();
            string verifyGuid = Guid.NewGuid().ToString();
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Sign and passwordCredentials: " + signAndPasswordGuid);
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Verify: " + verifyGuid);

            // Print out the password.
            Console.WriteLine("Password is: {0}", password);

            // Print out a displayName to use as an example.
            Console.WriteLine("displayName to use: CN=Example");
            Console.WriteLine();

            // Print out the public key.
            Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
            Console.WriteLine();

            // Generate the customKeyIdentifier using hash of thumbprint.
            Console.WriteLine("You can generate the customKeyIdentifier by getting the SHA256 hash of the certs thumprint.\nThe certs thumbprint is: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
            Console.WriteLine("The hash of the thumbprint that we will use for customeKeyIdentifier is:");
            string keyIdentifier = GetSha256FromThumbprint(selfsignedCert.Thumbprint);
            Console.WriteLine(keyIdentifier);
        }

        // Generate a self-signed certificate.
        private static X509Certificate2 buildSelfSignedServerCertificate(string password)
        {
            const string CertificateName = @"Microsoft Azure Federated SSO Certificate TEST";
            DateTime certificateStartDate = DateTime.UtcNow;
            DateTime certificateEndDate = certificateStartDate.AddYears(2).ToUniversalTime();

            X500DistinguishedName distinguishedName = new X500DistinguishedName($"CN={CertificateName}");

            using (RSA rsa = RSA.Create(2048))
            {
                var request = new CertificateRequest(distinguishedName, rsa, HashAlgorithmName.SHA256, RSASignaturePadding.Pkcs1);

                request.CertificateExtensions.Add(
                    new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false));

                var certificate = request.CreateSelfSigned(new DateTimeOffset(certificateStartDate), new DateTimeOffset(certificateEndDate));
                certificate.FriendlyName = CertificateName;

                return new X509Certificate2(certificate.Export(X509ContentType.Pfx, password), password, X509KeyStorageFlags.Exportable);
            }
        }

        // Generate hash from thumbprint.
        public static string GetSha256FromThumbprint(string thumbprint)
        {
            var message = Encoding.ASCII.GetBytes(thumbprint);
            SHA256Managed hashString = new SHA256Managed();
            return Convert.ToBase64String(hashString.ComputeHash(message));
        }
    }
}
```

### <a name="add-a-custom-signing-key"></a><span data-ttu-id="cd30c-242">添加自定义签名密钥</span><span class="sxs-lookup"><span data-stu-id="cd30c-242">Add a custom signing key</span></span>

<span data-ttu-id="cd30c-243">向服务主体添加以下信息：</span><span class="sxs-lookup"><span data-stu-id="cd30c-243">Add the following information to the service principal:</span></span>

* <span data-ttu-id="cd30c-244">私钥</span><span class="sxs-lookup"><span data-stu-id="cd30c-244">Private key</span></span>
* <span data-ttu-id="cd30c-245">密码</span><span class="sxs-lookup"><span data-stu-id="cd30c-245">Password</span></span>
* <span data-ttu-id="cd30c-246">公钥</span><span class="sxs-lookup"><span data-stu-id="cd30c-246">Public key</span></span> 

<span data-ttu-id="cd30c-247">从PFX文件中提取 Base64 编码公钥和私钥。</span><span class="sxs-lookup"><span data-stu-id="cd30c-247">Extract the private and public key Base64 encoded from the PFX file.</span></span> <span data-ttu-id="cd30c-248">要了解有关属性的更多信息，请参阅 [keyCredential 资源类型](/graph/api/resources/keycredential?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-248">To learn more about the properties, see [keyCredential resource type](/graph/api/resources/keycredential?view=graph-rest-1.0).</span></span>

<span data-ttu-id="cd30c-249">确保用于“签名”的 keyCredential 的keyId 与 passwordCredential 的 keyId 相匹配。</span><span class="sxs-lookup"><span data-stu-id="cd30c-249">Make sure that the keyId for the keyCredential used for "Sign" matches the keyId of the passwordCredential.</span></span> <span data-ttu-id="cd30c-250">可以通过获取证书指纹的哈希值来生成 `customkeyIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="cd30c-250">You can generate the `customkeyIdentifier` by getting the hash of the cert's thumbprint.</span></span> <span data-ttu-id="cd30c-251">请参阅前面的 C# 参考代码。</span><span class="sxs-lookup"><span data-stu-id="cd30c-251">See the previous C# reference code.</span></span>

#### <a name="request"></a><span data-ttu-id="cd30c-252">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-252">Request</span></span>

> [!NOTE]
> <span data-ttu-id="cd30c-253">为了提高可读性，keyCredentials 属性中的“项”值被缩短。</span><span class="sxs-lookup"><span data-stu-id="cd30c-253">The "key" value in the keyCredentials property is shortened for readability.</span></span> <span data-ttu-id="cd30c-254">该值为 base 64 编码。</span><span class="sxs-lookup"><span data-stu-id="cd30c-254">The value is base 64 encoded.</span></span> <span data-ttu-id="cd30c-255">对于私钥，属性 `usage` 是“签名”。</span><span class="sxs-lookup"><span data-stu-id="cd30c-255">For the private key the property `usage` is "Sign".</span></span> <span data-ttu-id="cd30c-256">对于公钥，属性 `usage` 是“验证”。</span><span class="sxs-lookup"><span data-stu-id="cd30c-256">For the public key the property `usage` is "Verify".</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "keyCredentials":[
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "X509CertAndPassword",
            "usage": "Sign",
            "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
            "displayName": "CN=awsAPI"
        },
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "AsymmetricX509Cert",
            "usage": "Verify",
            "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
            "displayName": "CN=awsAPI"
        }

    ],
    "passwordCredentials": [
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "endDateTime": "2022-01-27T19:40:33Z",
            "startDateTime": "2020-04-20T19:40:33Z",
            "secretText": "61891f4ee44d"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="cd30c-257">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-257">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="cd30c-258">激活自定义签名密钥</span><span class="sxs-lookup"><span data-stu-id="cd30c-258">Activate the custom signing key</span></span>

<span data-ttu-id="cd30c-259">需要将 `preferredTokenSigningKeyThumbprint` 属性设置为想要 Azure AD 用于签署 SAML 响应的证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="cd30c-259">You need to set the `preferredTokenSigningKeyThumbprint` property to the thumbprint of the certificate you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="cd30c-260">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-260">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "AC09FEF18DDE6983EE2A164FBA3C4DD7518BD787"
}
```

#### <a name="response"></a><span data-ttu-id="cd30c-261">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-261">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```
## <a name="step-5-assign-users"></a><span data-ttu-id="cd30c-262">第 5 步：分配用户</span><span class="sxs-lookup"><span data-stu-id="cd30c-262">Step 5: Assign users</span></span>

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="cd30c-263">向应用程序分配用户和组</span><span class="sxs-lookup"><span data-stu-id="cd30c-263">Assign users and groups to the application</span></span>

<span data-ttu-id="cd30c-264">将以下用户分配给服务主体，然后分配 AWS_Role1。</span><span class="sxs-lookup"><span data-stu-id="cd30c-264">Assign the following user to the service principal and assign the AWS_Role1.</span></span> 

| <span data-ttu-id="cd30c-265">名称</span><span class="sxs-lookup"><span data-stu-id="cd30c-265">Name</span></span>  | <span data-ttu-id="cd30c-266">ID</span><span class="sxs-lookup"><span data-stu-id="cd30c-266">ID</span></span>  |
|---------|---------|
| <span data-ttu-id="cd30c-267">用户 ID （principalId）</span><span class="sxs-lookup"><span data-stu-id="cd30c-267">User ID (principalId)</span></span> | <span data-ttu-id="cd30c-268">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span><span class="sxs-lookup"><span data-stu-id="cd30c-268">6cad4079-4e79-4a3f-9efb-ea30a14bdb26</span></span> |
| <span data-ttu-id="cd30c-269">类型（PrincipalType）</span><span class="sxs-lookup"><span data-stu-id="cd30c-269">Type (principalType)</span></span> | <span data-ttu-id="cd30c-270">用户</span><span class="sxs-lookup"><span data-stu-id="cd30c-270">User</span></span> |
| <span data-ttu-id="cd30c-271">应用程序角色 ID （appRoleId）</span><span class="sxs-lookup"><span data-stu-id="cd30c-271">App role ID (appRoleId)</span></span> | <span data-ttu-id="cd30c-272">454dc4c2-8176-498e-99df-8c4efcde41ef</span><span class="sxs-lookup"><span data-stu-id="cd30c-272">454dc4c2-8176-498e-99df-8c4efcde41ef</span></span> |
| <span data-ttu-id="cd30c-273">servicePrincipalID (resourceId)</span><span class="sxs-lookup"><span data-stu-id="cd30c-273">servicePrincipalID (resourceId)</span></span> | <span data-ttu-id="cd30c-274">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span><span class="sxs-lookup"><span data-stu-id="cd30c-274">f47a6776-bca7-4f2e-bc6c-eec59d058e3e</span></span> |

#### <a name="request"></a><span data-ttu-id="cd30c-275">请求</span><span class="sxs-lookup"><span data-stu-id="cd30c-275">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

#### <a name="response"></a><span data-ttu-id="cd30c-276">响应</span><span class="sxs-lookup"><span data-stu-id="cd30c-276">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
    "id": "rq7hyzl4yECaNZleMrTpDV-OCe5TEl5Ao_o76XMrRFU",
    "creationTimestamp": "2020-04-23T17:38:13.2508567Z",
    "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
    "principalDisplayName": "User 1",
    "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
    "principalType": "User",
    "resourceDisplayName": "AWS API Created",
    "resourceId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

<span data-ttu-id="cd30c-277">有关详细信息，请参阅 [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="cd30c-277">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0).</span></span>

## <a name="step-6-configure-the-application-side"></a><span data-ttu-id="cd30c-278">第 6 步：配置应用程序端</span><span class="sxs-lookup"><span data-stu-id="cd30c-278">Step 6: Configure the application side</span></span>

### <a name="get-azure-ad-saml-metadata"></a><span data-ttu-id="cd30c-279">获取 Azure AD SAML 元数据</span><span class="sxs-lookup"><span data-stu-id="cd30c-279">Get Azure AD SAML metadata</span></span>

<span data-ttu-id="cd30c-280">使用以下 URL 获取特定配置的应用程序的 Azure AD SAML 元数据。</span><span class="sxs-lookup"><span data-stu-id="cd30c-280">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="cd30c-281">元数据包含诸如签名证书、Azure AD entityID和 Azure AD SingleSignOnService 等信息。</span><span class="sxs-lookup"><span data-stu-id="cd30c-281">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

## <a name="next-steps"></a><span data-ttu-id="cd30c-282">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cd30c-282">Next steps</span></span>
- [<span data-ttu-id="cd30c-283">使用 Microsoft Graph API 配置用户预配</span><span class="sxs-lookup"><span data-stu-id="cd30c-283">Use Microsoft Graph APIs to configure user provisioning</span></span>](/azure/active-directory/app-provisioning/application-provisioning-configure-api)
- [<span data-ttu-id="cd30c-284">使用 AD FS 应用程序活动报告将应用程序迁移到 Azure AD</span><span class="sxs-lookup"><span data-stu-id="cd30c-284">Use the AD FS application activity report to migrate applications to Azure AD</span></span>](/azure/active-directory/manage-apps/migrate-adfs-application-activity)
