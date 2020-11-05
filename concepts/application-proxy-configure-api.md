---
title: 使用 Microsoft Graph Api 配置应用程序代理
description: 使用 Microsoft Graph Api 自动配置应用程序代理，以提供对本地应用程序的远程访问和单一登录。
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5052555b16b81170d8a6aa04f1c26c13fcd8d320
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921793"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="01fe5-103">使用 Microsoft Graph API 自动化应用程序代理的配置</span><span class="sxs-lookup"><span data-stu-id="01fe5-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="01fe5-104">在本文中，您将了解如何为应用程序创建和配置 Azure Active Directory (Azure AD) [应用程序代理](/azure/active-directory/manage-apps/what-is-application-proxy) 。</span><span class="sxs-lookup"><span data-stu-id="01fe5-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](/azure/active-directory/manage-apps/what-is-application-proxy) for an application.</span></span> <span data-ttu-id="01fe5-105">应用程序代理提供了对本地 web 应用程序的安全远程访问和单一登录。</span><span class="sxs-lookup"><span data-stu-id="01fe5-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="01fe5-106">为应用程序配置应用程序代理后，用户可以通过外部 URL、"我的应用程序" 门户或其他内部应用程序门户访问其本地应用程序。</span><span class="sxs-lookup"><span data-stu-id="01fe5-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="01fe5-107">本文假定您已经安装了连接器并完成了应用程序代理的 [先决条件](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) ，以便连接器可以与 Azure AD 服务进行通信。</span><span class="sxs-lookup"><span data-stu-id="01fe5-107">This article assumes you have already installed a connector and completed the [prerequisites](/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="01fe5-108">请确保你具有相应的权限来调用以下 API。</span><span class="sxs-lookup"><span data-stu-id="01fe5-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="01fe5-109">资源类型</span><span class="sxs-lookup"><span data-stu-id="01fe5-109">Resource type</span></span> |<span data-ttu-id="01fe5-110">方法</span><span class="sxs-lookup"><span data-stu-id="01fe5-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="01fe5-111">applications</span><span class="sxs-lookup"><span data-stu-id="01fe5-111">applications</span></span>](/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="01fe5-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="01fe5-112">onPremisesPublishing</span></span>](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="01fe5-113">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="01fe5-113">Create application</span></span>](/graph/api/application-post-applications?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="01fe5-114">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="01fe5-114">Update application</span></span>](/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="01fe5-115">向 connectorGroup 添加应用程序</span><span class="sxs-lookup"><span data-stu-id="01fe5-115">Add application to connectorGroup</span></span>](/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="01fe5-116">connector</span><span class="sxs-lookup"><span data-stu-id="01fe5-116">connector</span></span>](/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="01fe5-117">获取连接器</span><span class="sxs-lookup"><span data-stu-id="01fe5-117">Get connectors</span></span>](/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="01fe5-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="01fe5-118">connectorGroup</span></span>](/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="01fe5-119">Create connectorGroup</span><span class="sxs-lookup"><span data-stu-id="01fe5-119">Create connectorGroup</span></span>](/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="01fe5-120">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="01fe5-120">Add connector to connectorGroup</span></span>](/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="01fe5-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="01fe5-121">servicePrincipals</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="01fe5-122">创建 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="01fe5-122">Create servicePrincipal</span></span>](/graph/api/serviceprincipal-post-serviceprincipals?tabs=http&view=graph-rest-beta) <br> [<span data-ttu-id="01fe5-123">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="01fe5-123">Update servicePrincipal</span></span>](/graph/api/serviceprincipal-update?tabs=http&view=graph-rest-1.0) <br> [<span data-ttu-id="01fe5-124">创建 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="01fe5-124">Create appRoleAssignments</span></span>](/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="01fe5-125">本文中所示的请求使用示例值。</span><span class="sxs-lookup"><span data-stu-id="01fe5-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="01fe5-126">你将需要更新这些。</span><span class="sxs-lookup"><span data-stu-id="01fe5-126">You will need update these.</span></span> <span data-ttu-id="01fe5-127">显示的响应对象可能还会缩短可读性。</span><span class="sxs-lookup"><span data-stu-id="01fe5-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="01fe5-128">步骤1：创建应用程序</span><span class="sxs-lookup"><span data-stu-id="01fe5-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="01fe5-129">登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端</span><span class="sxs-lookup"><span data-stu-id="01fe5-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="01fe5-130">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="01fe5-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="01fe5-131">选择 **"使用 Microsoft 登录"** ，并使用 Azure AD 全局管理员或应用程序管理员凭据登录。</span><span class="sxs-lookup"><span data-stu-id="01fe5-131">Select **Sign-in with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="01fe5-132">成功登录后，将在左窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="01fe5-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

### <a name="create-an-application"></a><span data-ttu-id="01fe5-133">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="01fe5-133">Create an application</span></span>

<span data-ttu-id="01fe5-134">若要使用 API 为应用程序配置应用程序代理，请创建应用程序，将服务主体添加到应用中，然后更新应用程序的 **onPremisesPublishing** 属性以配置应用程序代理设置。</span><span class="sxs-lookup"><span data-stu-id="01fe5-134">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="01fe5-135">在创建应用程序时，将应用程序的 **signInAudience** 设置为 "AzureADMyOrg"。</span><span class="sxs-lookup"><span data-stu-id="01fe5-135">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-136">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01fe5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fe5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications
Content-type: application/json

{
  "displayName": "Contoso IWA App",
  "signInAudience":"AzureADMyOrg"
}
```
# <a name="c"></a>[<span data-ttu-id="01fe5-138">C#</span><span class="sxs-lookup"><span data-stu-id="01fe5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01fe5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fe5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01fe5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01fe5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01fe5-141">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "deletedDateTime": null,
  "addIns": [],
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "identifierUris": [],
  "createdDateTime": "2020-08-11T21:07:47.5919755Z",
  "description": null,
  "displayName": "Contoso IWA App",
  "isAuthorizationServiceEnabled": false,
  "isDeviceOnlyAuthSupported": null,
  "isFallbackPublicClient": null,
  "groupMembershipClaims": null,
  "notes": null,
  "optionalClaims": null,
  "orgRestrictions": [],
  "publisherDomain": "f128.info",
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null,
  "uniqueName": null,
  "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
  },
}
```

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="01fe5-142">检索应用程序对象 ID 和 appId</span><span class="sxs-lookup"><span data-stu-id="01fe5-142">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="01fe5-143">使用上一次调用的响应检索并保存应用程序对象 ID 和应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="01fe5-143">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="01fe5-144">为应用程序创建一个 servicePrincipal 并添加所需的标记</span><span class="sxs-lookup"><span data-stu-id="01fe5-144">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="01fe5-145">使用 **appId** 为应用程序创建服务主体。</span><span class="sxs-lookup"><span data-stu-id="01fe5-145">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="01fe5-146">然后添加为应用配置应用程序代理所需的标记。</span><span class="sxs-lookup"><span data-stu-id="01fe5-146">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-147">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01fe5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fe5-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_servicePrincipal"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: appplication/json

{
  "appId":"d7fbfe28-c60e-46d2-8335-841923950d3b",
  "tags": [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="01fe5-149">C#</span><span class="sxs-lookup"><span data-stu-id="01fe5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01fe5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fe5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01fe5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01fe5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01fe5-152">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
  "id": "a8cac399-cde5-4516-a674-819503c61313",
  "deletedDateTime": null,
  "accountEnabled": true,
  "alternativeNames": [],
  "createdDateTime": null,
  "deviceManagementAppType": null,
  "appDescription": null,
  "appDisplayName": "Contoso IWA App",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "appOwnerOrganizationId": "7918d4b5-0442-4a97-be2d-36f9f9962ece",
  "appRoleAssignmentRequired": false,
  "description": null,
  "displayName": "vtestapi2",
  "errorUrl": null,
  "homepage": null,
  "isAuthorizationServiceEnabled": false,
  "loginUrl": null,
  "logoutUrl": null,
  "notes": null,
  "notificationEmailAddresses": [],
  "preferredSingleSignOnMode": null,
  "preferredTokenSigningKeyEndDateTime": null,
  "preferredTokenSigningKeyThumbprint": null,
  "publisherName": "f/128 Photography",
  "replyUrls": [],
  "samlMetadataUrl": null,
  "samlSingleSignOnSettings": null,
  "servicePrincipalNames": [
      "b92b92d4-3874-46a5-b715-a00ea01cff93"
  ],
  "servicePrincipalType": "Application",
}
```

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="01fe5-153">步骤2：配置应用程序代理属性</span><span class="sxs-lookup"><span data-stu-id="01fe5-153">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="01fe5-154">设置 onPremisesPublishing 配置</span><span class="sxs-lookup"><span data-stu-id="01fe5-154">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="01fe5-155">使用上一步中的 application 对象 ID 为应用程序配置应用程序代理，并将 **onPremisesPublishing** 属性更新为所需的配置。</span><span class="sxs-lookup"><span data-stu-id="01fe5-155">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="01fe5-156">在此示例中，您使用的是内部 URL 的应用程序： `https://contosoiwaapp.com` 并使用外部 url 的默认域： `https://contosoiwaapp-contoso.msappproxy.net` 。</span><span class="sxs-lookup"><span data-stu-id="01fe5-156">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="01fe5-157">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01fe5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fe5-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
    "onPremisesPublishing": {
        "externalAuthenticationType": "aadPreAuthentication",
        "internalUrl": "https://contosoiwaapp.com",
        "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="01fe5-159">C#</span><span class="sxs-lookup"><span data-stu-id="01fe5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01fe5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fe5-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01fe5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01fe5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01fe5-162">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="01fe5-163">完成应用程序的配置</span><span class="sxs-lookup"><span data-stu-id="01fe5-163">Complete the configuration of the application</span></span>
<span data-ttu-id="01fe5-164">将应用程序的 " **redirectUri** "、" **identifierUri** " 和 " **HomepageUrl** " 属性更新为 **onPremisesPublishing** 属性中配置的外部 UR。</span><span class="sxs-lookup"><span data-stu-id="01fe5-164">Update the application's **redirectUri** , **identifierUri** , and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="01fe5-165">然后，将 [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) 更新为 `true` 针对 **enabledTokenIssuance** 和 `false` **enabledAccessTokenIssuance** 。</span><span class="sxs-lookup"><span data-stu-id="01fe5-165">Then update [implicitGrantSettings](/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-166">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-166">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
  "identifierUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
  "web": {
    "redirectUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
    "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net",
    "implicitGrantSettings": {
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": false
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="01fe5-167">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-167">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="01fe5-168">步骤3：将连接器组分配给应用程序</span><span class="sxs-lookup"><span data-stu-id="01fe5-168">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="01fe5-169">获取连接器</span><span class="sxs-lookup"><span data-stu-id="01fe5-169">Get connectors</span></span>

<span data-ttu-id="01fe5-170">列出连接器并使用响应来检索和保存连接器对象 ID。</span><span class="sxs-lookup"><span data-stu-id="01fe5-170">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="01fe5-171">连接器对象 ID 将用于将连接器分配给连接器组。</span><span class="sxs-lookup"><span data-stu-id="01fe5-171">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-172">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-172">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01fe5-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fe5-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="01fe5-174">C#</span><span class="sxs-lookup"><span data-stu-id="01fe5-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01fe5-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fe5-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01fe5-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01fe5-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01fe5-177">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-177">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectors",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectors",
    "value": [
        {
            "id": "d2b1e8e8-8511-49d6-a4ba-323cb083fbb0",
            "machineName": "connectorA.redmond.contoso.com"",
            "externalIp": "131.137.147.164",
            "status": "active"
        },
        {
            "id": "f2cab422-a1c8-4d70-a47e-2cb297a2e051",
            "machineName": "connectorB.contoso.com"",
            "externalIp": "68.0.191.210",
            "status": "active"
        },
        {
            "id": "8555cc3c-5c8b-48a8-a8b2-5e97c32ef907",
            "machineName": "connectorC.contoso.com",
            "externalIp": "40.78.66.161",
            "status": "active"
        }
    ]
}
```

### <a name="create-a-connectorgroup"></a><span data-ttu-id="01fe5-178">创建 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="01fe5-178">Create a connectorGroup</span></span>
<span data-ttu-id="01fe5-179">在此示例中，创建了一个用于应用程序的名为 "IWA Demo Connector Group" 的新 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="01fe5-179">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="01fe5-180">如果您的连接器已分配给相应的 connectorGroup，也可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="01fe5-180">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="01fe5-181">检索并保存要在下一步中使用的 connectorGroup 对象 ID。</span><span class="sxs-lookup"><span data-stu-id="01fe5-181">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-182">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-182">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
   "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a><span data-ttu-id="01fe5-183">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-183">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 201
Content-type: connectorGroup/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectorGroups/$entity",
    "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
    "name": "IWA Demo Connector Group",
    "connectorGroupType": "applicationProxy",
    "isDefault": false
}
```

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="01fe5-184">将连接器分配给 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="01fe5-184">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-185">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-185">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/8555cc3c-5c8b-48a8-a8b2-5e97c32ef907/memberOf/$ref

Content-type: application/json
{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a><span data-ttu-id="01fe5-186">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="01fe5-187">将应用程序分配给 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="01fe5-187">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-188">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-188">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01fe5-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fe5-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```
# <a name="c"></a>[<span data-ttu-id="01fe5-190">C#</span><span class="sxs-lookup"><span data-stu-id="01fe5-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01fe5-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fe5-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01fe5-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01fe5-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01fe5-193">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-193">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="01fe5-194">步骤4：配置单一登录</span><span class="sxs-lookup"><span data-stu-id="01fe5-194">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="01fe5-195">此应用程序使用集成的 Windows 身份验证 (IWA) 。</span><span class="sxs-lookup"><span data-stu-id="01fe5-195">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="01fe5-196">若要配置 IWA，请在 [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) 资源类型中设置单一登录属性。</span><span class="sxs-lookup"><span data-stu-id="01fe5-196">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-197">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-197">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
   "onPremisesPublishing": {
      "singleSignOnSettings": {
         "kerberosSignOnSettings": {
            "kerberosServicePrincipalName": "HTTP/iwademo.contoso.com",
        "kerberosSignOnMappingAttributeType": "userPrincipalName"
         },
         "singleSignOnMode": "onPremisesKerberos"
      }
   }
}
```

#### <a name="response"></a><span data-ttu-id="01fe5-198">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-198">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="01fe5-199">第 5 步：分配用户</span><span class="sxs-lookup"><span data-stu-id="01fe5-199">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="01fe5-200">检索应用程序的 appRole</span><span class="sxs-lookup"><span data-stu-id="01fe5-200">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="01fe5-201">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-201">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="01fe5-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fe5-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```
# <a name="c"></a>[<span data-ttu-id="01fe5-203">C#</span><span class="sxs-lookup"><span data-stu-id="01fe5-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01fe5-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fe5-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01fe5-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01fe5-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="01fe5-206">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-206">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('a8cac399-cde5-4516-a674-819503c61313')/appRoles",
    "value": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "b9632174-c057-4f7e-951b-be3adc52bfe6",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        }
    ]
}
```

<span data-ttu-id="01fe5-207">使用上一次调用中的响应检索并保存 appRole ID 以用于下一步。</span><span class="sxs-lookup"><span data-stu-id="01fe5-207">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="01fe5-208">向应用程序分配用户和组</span><span class="sxs-lookup"><span data-stu-id="01fe5-208">Assign users and groups to the application</span></span>

<span data-ttu-id="01fe5-209">使用以下属性将用户分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="01fe5-209">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="01fe5-210">属性</span><span class="sxs-lookup"><span data-stu-id="01fe5-210">Property</span></span>  | <span data-ttu-id="01fe5-211">说明</span><span class="sxs-lookup"><span data-stu-id="01fe5-211">Description</span></span> |<span data-ttu-id="01fe5-212">ID</span><span class="sxs-lookup"><span data-stu-id="01fe5-212">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="01fe5-213">principalId</span><span class="sxs-lookup"><span data-stu-id="01fe5-213">principalId</span></span> | <span data-ttu-id="01fe5-214">将分配给应用程序的用户的用户 ID</span><span class="sxs-lookup"><span data-stu-id="01fe5-214">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="01fe5-215">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="01fe5-215">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="01fe5-216">principalType</span><span class="sxs-lookup"><span data-stu-id="01fe5-216">principalType</span></span> | <span data-ttu-id="01fe5-217">用户类型</span><span class="sxs-lookup"><span data-stu-id="01fe5-217">Type of user</span></span> | <span data-ttu-id="01fe5-218">用户</span><span class="sxs-lookup"><span data-stu-id="01fe5-218">User</span></span> |
| <span data-ttu-id="01fe5-219">appRoleId</span><span class="sxs-lookup"><span data-stu-id="01fe5-219">appRoleId</span></span> |  <span data-ttu-id="01fe5-220">应用程序的默认应用程序角色的应用程序角色 ID</span><span class="sxs-lookup"><span data-stu-id="01fe5-220">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="01fe5-221">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="01fe5-221">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="01fe5-222">resourceId</span><span class="sxs-lookup"><span data-stu-id="01fe5-222">resourceId</span></span> | <span data-ttu-id="01fe5-223">应用程序的 servicePrincipal ID</span><span class="sxs-lookup"><span data-stu-id="01fe5-223">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="01fe5-224">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="01fe5-224">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="01fe5-225">请求</span><span class="sxs-lookup"><span data-stu-id="01fe5-225">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a><span data-ttu-id="01fe5-226">响应</span><span class="sxs-lookup"><span data-stu-id="01fe5-226">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
    "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
    "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
    "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
    "principalDisplayName": "Jean Green",
    "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
    "principalType": "User",
    "resourceDisplayName": "Contoso IWA App",
    "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```

<span data-ttu-id="01fe5-227">有关详细信息，请参阅 [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="01fe5-227">For more information, see [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="01fe5-228">其他步骤</span><span class="sxs-lookup"><span data-stu-id="01fe5-228">Additional steps</span></span>
- [<span data-ttu-id="01fe5-229">使用 PowerShell 示例为应用程序代理自动执行配置</span><span class="sxs-lookup"><span data-stu-id="01fe5-229">Automate configuration using PowerShell samples for Application Proxy</span></span>](/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="01fe5-230">使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置</span><span class="sxs-lookup"><span data-stu-id="01fe5-230">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)