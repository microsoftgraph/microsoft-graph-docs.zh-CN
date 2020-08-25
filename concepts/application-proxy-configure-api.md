---
title: 使用 Microsoft Graph Api 配置应用程序代理
description: 使用 Microsoft Graph Api 自动配置应用程序代理，以提供对本地应用程序的远程访问和单一登录。
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc99857905a0a308f49ddc41bf22da993ca8f1b4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873102"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="d860b-103">使用 Microsoft Graph API 自动配置应用程序代理</span><span class="sxs-lookup"><span data-stu-id="d860b-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="d860b-104">在本文中，您将了解如何为应用程序创建和配置 Azure Active Directory (Azure AD) [应用程序代理](https://aka.ms/whyappproxy) 。</span><span class="sxs-lookup"><span data-stu-id="d860b-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="d860b-105">应用程序代理提供了对本地 web 应用程序的安全远程访问和单一登录。</span><span class="sxs-lookup"><span data-stu-id="d860b-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="d860b-106">为应用程序配置应用程序代理后，用户可以通过外部 URL、"我的应用程序" 门户或其他内部应用程序门户访问其本地应用程序。</span><span class="sxs-lookup"><span data-stu-id="d860b-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="d860b-107">本文假定您已经安装了连接器并完成了应用程序代理的 [先决条件](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) ，以便连接器可以与 Azure AD 服务进行通信。</span><span class="sxs-lookup"><span data-stu-id="d860b-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="d860b-108">请确保你具有相应的权限来调用以下 API。</span><span class="sxs-lookup"><span data-stu-id="d860b-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="d860b-109">资源类型</span><span class="sxs-lookup"><span data-stu-id="d860b-109">Resource type</span></span> |<span data-ttu-id="d860b-110">方法</span><span class="sxs-lookup"><span data-stu-id="d860b-110">Method</span></span> |
|---------|---------|
|[<span data-ttu-id="d860b-111">applications</span><span class="sxs-lookup"><span data-stu-id="d860b-111">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="d860b-112">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="d860b-112">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [<span data-ttu-id="d860b-113">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="d860b-113">Create application</span></span>](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="d860b-114">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="d860b-114">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="d860b-115">向 connectorGroup 添加应用程序</span><span class="sxs-lookup"><span data-stu-id="d860b-115">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="d860b-116">连接器</span><span class="sxs-lookup"><span data-stu-id="d860b-116">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="d860b-117">获取连接器</span><span class="sxs-lookup"><span data-stu-id="d860b-117">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="d860b-118">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d860b-118">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="d860b-119">Create connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d860b-119">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="d860b-120">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d860b-120">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="d860b-121">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="d860b-121">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="d860b-122">创建 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="d860b-122">Create servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [<span data-ttu-id="d860b-123">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="d860b-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="d860b-124">创建 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="d860b-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> <span data-ttu-id="d860b-125">本文中所示的请求使用示例值。</span><span class="sxs-lookup"><span data-stu-id="d860b-125">The requests shown in this article use sample values.</span></span> <span data-ttu-id="d860b-126">你将需要更新这些。</span><span class="sxs-lookup"><span data-stu-id="d860b-126">You will need update these.</span></span> <span data-ttu-id="d860b-127">显示的响应对象可能还会缩短可读性。</span><span class="sxs-lookup"><span data-stu-id="d860b-127">The response objects shown might also be shortened for readability.</span></span> 

## <a name="step-1-create-an-application"></a><span data-ttu-id="d860b-128">步骤1：创建应用程序</span><span class="sxs-lookup"><span data-stu-id="d860b-128">Step 1: Create an application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="d860b-129">登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端</span><span class="sxs-lookup"><span data-stu-id="d860b-129">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="d860b-130">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="d860b-130">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="d860b-131">选择 **"使用 Microsoft 登录"** ，并使用 Azure AD 全局管理员或应用程序管理员凭据登录。</span><span class="sxs-lookup"><span data-stu-id="d860b-131">Select **Sign-in with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="d860b-132">成功登录后，将在左窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="d860b-132">Upon successful sign in, you'll see the user account details in the left pane.</span></span>

### <a name="create-an-application"></a><span data-ttu-id="d860b-133">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="d860b-133">Create an application</span></span>

<span data-ttu-id="d860b-134">若要使用 API 为应用程序配置应用程序代理，请创建应用程序，将服务主体添加到应用中，然后更新应用程序的 **onPremisesPublishing** 属性以配置应用程序代理设置。</span><span class="sxs-lookup"><span data-stu-id="d860b-134">To configure Application Proxy for an app using the API, you create an application, add a service principal to the app, and then update the application's **onPremisesPublishing** property to configure the App Proxy settings.</span></span> <span data-ttu-id="d860b-135">在创建应用程序时，将应用程序的 **signInAudience** 设置为 "AzureADMyOrg"。</span><span class="sxs-lookup"><span data-stu-id="d860b-135">When creating the application, set the application's **signInAudience** to "AzureADMyOrg".</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-136">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-136">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-137">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-137">Response</span></span>

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

### <a name="retrieve-the-application-object-id-and-appid"></a><span data-ttu-id="d860b-138">检索应用程序对象 ID 和 appId</span><span class="sxs-lookup"><span data-stu-id="d860b-138">Retrieve the application object ID and appId</span></span>
<span data-ttu-id="d860b-139">使用上一次调用的响应检索并保存应用程序对象 ID 和应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="d860b-139">Use the response from the previous call to retrieve and save the application object ID and app ID.</span></span>
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a><span data-ttu-id="d860b-140">为应用程序创建一个 servicePrincipal 并添加所需的标记</span><span class="sxs-lookup"><span data-stu-id="d860b-140">Create a servicePrincipal for the application and add required tags</span></span>
<span data-ttu-id="d860b-141">使用 **appId** 为应用程序创建服务主体。</span><span class="sxs-lookup"><span data-stu-id="d860b-141">Use the **appId** to create a service principal for the application.</span></span> <span data-ttu-id="d860b-142">然后添加为应用配置应用程序代理所需的标记。</span><span class="sxs-lookup"><span data-stu-id="d860b-142">Then add the tags required for configuring Application Proxy for an app.</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-143">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-143">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-144">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-144">Response</span></span>
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

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="d860b-145">步骤2：配置应用程序代理属性</span><span class="sxs-lookup"><span data-stu-id="d860b-145">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="d860b-146">设置 onPremisesPublishing 配置</span><span class="sxs-lookup"><span data-stu-id="d860b-146">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="d860b-147">使用上一步中的 application 对象 ID 为应用程序配置应用程序代理，并将 **onPremisesPublishing** 属性更新为所需的配置。</span><span class="sxs-lookup"><span data-stu-id="d860b-147">Use the application object ID from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="d860b-148">在此示例中，您使用的是内部 URL 的应用程序： `https://contosoiwaapp.com` 并使用外部 url 的默认域： `https://contosoiwaapp-contoso.msappproxy.net` 。</span><span class="sxs-lookup"><span data-stu-id="d860b-148">In this example, you're using an app with the internal URL: `https://contosoiwaapp.com` and using the default domain for the external URL: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="d860b-149">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-149">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-150">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a><span data-ttu-id="d860b-151">完成应用程序的配置</span><span class="sxs-lookup"><span data-stu-id="d860b-151">Complete the configuration of the application</span></span>
<span data-ttu-id="d860b-152">将应用程序的 " **redirectUri**"、" **identifierUri**" 和 " **HomepageUrl** " 属性更新为 **onPremisesPublishing** 属性中配置的外部 UR。</span><span class="sxs-lookup"><span data-stu-id="d860b-152">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** properties to the external UR configured in the **onPremisesPublishing** property.</span></span> <span data-ttu-id="d860b-153">然后，将 [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) 更新为 `true` 针对 **enabledTokenIssuance** 和 `false` **enabledAccessTokenIssuance**。</span><span class="sxs-lookup"><span data-stu-id="d860b-153">Then update [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) to `true` for **enabledTokenIssuance** and `false` for **enabledAccessTokenIssuance**.</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-154">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-154">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="d860b-155">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="d860b-156">步骤3：将连接器组分配给应用程序</span><span class="sxs-lookup"><span data-stu-id="d860b-156">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="d860b-157">获取连接器</span><span class="sxs-lookup"><span data-stu-id="d860b-157">Get connectors</span></span>

<span data-ttu-id="d860b-158">列出连接器并使用响应来检索和保存连接器对象 ID。</span><span class="sxs-lookup"><span data-stu-id="d860b-158">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="d860b-159">连接器对象 ID 将用于将连接器分配给连接器组。</span><span class="sxs-lookup"><span data-stu-id="d860b-159">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-160">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```

#### <a name="response"></a><span data-ttu-id="d860b-161">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-161">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="d860b-162">创建 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d860b-162">Create a connectorGroup</span></span>
<span data-ttu-id="d860b-163">在此示例中，创建了一个用于应用程序的名为 "IWA Demo Connector Group" 的新 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="d860b-163">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="d860b-164">如果您的连接器已分配给相应的 connectorGroup，也可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="d860b-164">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="d860b-165">检索并保存要在下一步中使用的 connectorGroup 对象 ID。</span><span class="sxs-lookup"><span data-stu-id="d860b-165">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-166">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-166">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-167">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-167">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="d860b-168">将连接器分配给 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d860b-168">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-169">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-169">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-170">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-170">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="d860b-171">将应用程序分配给 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="d860b-171">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-172">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-172">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-173">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-173">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="d860b-174">步骤4：配置单一登录</span><span class="sxs-lookup"><span data-stu-id="d860b-174">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="d860b-175">此应用程序使用集成的 Windows 身份验证 (IWA) 。</span><span class="sxs-lookup"><span data-stu-id="d860b-175">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="d860b-176">若要配置 IWA，请在 [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) 资源类型中设置单一登录属性。</span><span class="sxs-lookup"><span data-stu-id="d860b-176">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-177">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-177">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-178">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-178">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="d860b-179">第 5 步：分配用户</span><span class="sxs-lookup"><span data-stu-id="d860b-179">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="d860b-180">检索应用程序的 appRole</span><span class="sxs-lookup"><span data-stu-id="d860b-180">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="d860b-181">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-181">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a><span data-ttu-id="d860b-182">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-182">Response</span></span>

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

<span data-ttu-id="d860b-183">使用上一次调用中的响应检索并保存 appRole ID 以用于下一步。</span><span class="sxs-lookup"><span data-stu-id="d860b-183">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="d860b-184">向应用程序分配用户和组</span><span class="sxs-lookup"><span data-stu-id="d860b-184">Assign users and groups to the application</span></span>

<span data-ttu-id="d860b-185">使用以下属性将用户分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="d860b-185">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="d860b-186">属性</span><span class="sxs-lookup"><span data-stu-id="d860b-186">Property</span></span>  | <span data-ttu-id="d860b-187">说明</span><span class="sxs-lookup"><span data-stu-id="d860b-187">Description</span></span> |<span data-ttu-id="d860b-188">ID</span><span class="sxs-lookup"><span data-stu-id="d860b-188">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="d860b-189">principalId</span><span class="sxs-lookup"><span data-stu-id="d860b-189">principalId</span></span> | <span data-ttu-id="d860b-190">将分配给应用程序的用户的用户 ID</span><span class="sxs-lookup"><span data-stu-id="d860b-190">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="d860b-191">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="d860b-191">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="d860b-192">principalType</span><span class="sxs-lookup"><span data-stu-id="d860b-192">principalType</span></span> | <span data-ttu-id="d860b-193">用户类型</span><span class="sxs-lookup"><span data-stu-id="d860b-193">Type of user</span></span> | <span data-ttu-id="d860b-194">用户</span><span class="sxs-lookup"><span data-stu-id="d860b-194">User</span></span> |
| <span data-ttu-id="d860b-195">appRoleId</span><span class="sxs-lookup"><span data-stu-id="d860b-195">appRoleId</span></span> |  <span data-ttu-id="d860b-196">应用程序的默认应用程序角色的应用程序角色 ID</span><span class="sxs-lookup"><span data-stu-id="d860b-196">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="d860b-197">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="d860b-197">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="d860b-198">resourceId</span><span class="sxs-lookup"><span data-stu-id="d860b-198">resourceId</span></span> | <span data-ttu-id="d860b-199">应用程序的 servicePrincipal ID</span><span class="sxs-lookup"><span data-stu-id="d860b-199">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="d860b-200">a8cac399-cde5-4516-a674-819503c61313</span><span class="sxs-lookup"><span data-stu-id="d860b-200">a8cac399-cde5-4516-a674-819503c61313</span></span> |

#### <a name="request"></a><span data-ttu-id="d860b-201">请求</span><span class="sxs-lookup"><span data-stu-id="d860b-201">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d860b-202">响应</span><span class="sxs-lookup"><span data-stu-id="d860b-202">Response</span></span>

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

<span data-ttu-id="d860b-203">有关详细信息，请参阅 [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="d860b-203">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>


## <a name="additional-steps"></a><span data-ttu-id="d860b-204">其他步骤</span><span class="sxs-lookup"><span data-stu-id="d860b-204">Additional steps</span></span>
- [<span data-ttu-id="d860b-205">使用 PowerShell 示例为应用程序代理自动执行配置</span><span class="sxs-lookup"><span data-stu-id="d860b-205">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="d860b-206">使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置</span><span class="sxs-lookup"><span data-stu-id="d860b-206">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
