---
title: 使用 Microsoft Graph Api 配置应用程序代理
description: 使用 Microsoft Graph Api 自动配置应用程序代理，以提供对本地应用程序的远程访问和单一登录。
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 11ce7e7388ce6ab8b17244dbe964ff99cbeaf539
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658054"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a><span data-ttu-id="92efe-103">使用 Microsoft Graph API 自动配置应用程序代理</span><span class="sxs-lookup"><span data-stu-id="92efe-103">Automate the configuration of Application Proxy using the Microsoft Graph API</span></span>

<span data-ttu-id="92efe-104">在本文中，您将了解如何为应用程序创建和配置 Azure Active Directory (Azure AD) [应用程序代理](https://aka.ms/whyappproxy) 。</span><span class="sxs-lookup"><span data-stu-id="92efe-104">In this article, you'll learn how to create and configure Azure Active Directory (Azure AD) [Application Proxy](https://aka.ms/whyappproxy) for an application.</span></span> <span data-ttu-id="92efe-105">应用程序代理提供了对本地 web 应用程序的安全远程访问和单一登录。</span><span class="sxs-lookup"><span data-stu-id="92efe-105">Application Proxy provides secure remote access and single sign-on to on-premises web applications.</span></span> <span data-ttu-id="92efe-106">为应用程序配置应用程序代理后，用户可以通过外部 URL、"我的应用程序" 门户或其他内部应用程序门户访问其本地应用程序。</span><span class="sxs-lookup"><span data-stu-id="92efe-106">After configuring Application Proxy for an application, users can access their on-premises applications through an external URL, the My Apps portal, or other internal application portals.</span></span>

<span data-ttu-id="92efe-107">本文假定您已经安装了连接器并完成了应用程序代理的 [先决条件](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) ，以便连接器可以与 Azure AD 服务进行通信。</span><span class="sxs-lookup"><span data-stu-id="92efe-107">This article assumes you have already installed a connector and completed the [prerequisites](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) for Application Proxy so that connectors can communicate with Azure AD services.</span></span>

<span data-ttu-id="92efe-108">请确保你具有相应的权限来调用以下 API。</span><span class="sxs-lookup"><span data-stu-id="92efe-108">Make sure you have the corresponding permissions to call the following APIs.</span></span>

|<span data-ttu-id="92efe-109">资源类型</span><span class="sxs-lookup"><span data-stu-id="92efe-109">Resource type</span></span> |<span data-ttu-id="92efe-110">方法</span><span class="sxs-lookup"><span data-stu-id="92efe-110">Method</span></span> |
|---------|---------|
| [<span data-ttu-id="92efe-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="92efe-111">applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)| [<span data-ttu-id="92efe-112">实例化 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="92efe-112">Instantiate applicationTemplate</span></span>](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) |
|[<span data-ttu-id="92efe-113">applications</span><span class="sxs-lookup"><span data-stu-id="92efe-113">applications</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [<span data-ttu-id="92efe-114">onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="92efe-114">onPremisesPublishing</span></span>](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)|[<span data-ttu-id="92efe-115">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="92efe-115">Update application</span></span>](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [<span data-ttu-id="92efe-116">向 connectorGroup 添加应用程序</span><span class="sxs-lookup"><span data-stu-id="92efe-116">Add application to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[<span data-ttu-id="92efe-117">连接器</span><span class="sxs-lookup"><span data-stu-id="92efe-117">connector</span></span>](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [<span data-ttu-id="92efe-118">获取连接器</span><span class="sxs-lookup"><span data-stu-id="92efe-118">Get connectors</span></span>](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[<span data-ttu-id="92efe-119">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="92efe-119">connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [<span data-ttu-id="92efe-120">Create connectorGroup</span><span class="sxs-lookup"><span data-stu-id="92efe-120">Create connectorGroup</span></span>](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [<span data-ttu-id="92efe-121">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="92efe-121">Add connector to connectorGroup</span></span>](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[<span data-ttu-id="92efe-122">servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="92efe-122">servicePrincipals</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[<span data-ttu-id="92efe-123">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="92efe-123">Update servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [<span data-ttu-id="92efe-124">创建 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="92efe-124">Create appRoleAssignments</span></span>](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

>[!NOTE]
> <span data-ttu-id="92efe-125">本文中所示的请求使用示例值。</span><span class="sxs-lookup"><span data-stu-id="92efe-125">The requests shown in this article uses sample values.</span></span> <span data-ttu-id="92efe-126">你将需要更新这些。</span><span class="sxs-lookup"><span data-stu-id="92efe-126">You will need update these.</span></span> <span data-ttu-id="92efe-127">为了提高可读性，还可能缩短了显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="92efe-127">The response objects shown may also be shortened for readability.</span></span> <span data-ttu-id="92efe-128">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92efe-128">All the properties will be returned from an actual call.</span></span>

## <a name="step-1-create-a-custom-application"></a><span data-ttu-id="92efe-129">步骤1：创建自定义应用程序</span><span class="sxs-lookup"><span data-stu-id="92efe-129">Step 1: Create a custom application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="92efe-130">登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端</span><span class="sxs-lookup"><span data-stu-id="92efe-130">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="92efe-131">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="92efe-131">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="92efe-132">选择**使用 Microsoft 登录**，然后使用 Azure AD 全局管理员或 App Admin 凭据登录。</span><span class="sxs-lookup"><span data-stu-id="92efe-132">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator or App Admin credentials.</span></span>
3. <span data-ttu-id="92efe-133">登录成功后，将在左窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="92efe-133">Upon successful sign-in, you'll see the user account details in the left pane.</span></span>

### <a name="create-a-custom-application"></a><span data-ttu-id="92efe-134">创建自定义应用程序</span><span class="sxs-lookup"><span data-stu-id="92efe-134">Create a custom application</span></span>

<span data-ttu-id="92efe-135">若要使用 API 为应用程序配置应用程序代理，您必须首先创建自定义应用程序，然后更新应用程序的 **onPremisesPublishing** 属性，以配置应用程序代理设置。</span><span class="sxs-lookup"><span data-stu-id="92efe-135">To configure Application Proxy for an app using the API, you must first create a custom application, then update the application's **onPremisesPublishing** property for the app to configure the App Proxy settings.</span></span>
<span data-ttu-id="92efe-136">使用 [实例化 applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) 在租户中创建自定义应用程序和服务主体的实例，以供管理。</span><span class="sxs-lookup"><span data-stu-id="92efe-136">Use [instantiate applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) to create an instance of a custom application and service principal in your tenant for management.</span></span> <span data-ttu-id="92efe-137">自定义应用程序的模板 ID 为： `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` 。</span><span class="sxs-lookup"><span data-stu-id="92efe-137">The template ID for a custom application is: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-138">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="92efe-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="92efe-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_applicationTemplate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
  "displayName": "Contoso IWA App"
}
```
# <a name="c"></a>[<span data-ttu-id="92efe-140">C#</span><span class="sxs-lookup"><span data-stu-id="92efe-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92efe-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92efe-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92efe-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92efe-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="92efe-143">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-143">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "displayName": "Contoso IWA App",
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "identifierUris": [],
        "publicClient": null,
        "replyUrls": [],
        "logoutUrl": null,
        "samlMetadataUrl": null,
        "errorUrl": null,
        "groupMembershipClaims": null,
        "availableToOtherTenants": false
    },
    "servicePrincipal": {
        "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea",
        "deletionTimestamp": null,
        "accountEnabled": true,
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "appDisplayName": "Contoso API",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "appRoleAssignmentRequired": true,
        "displayName": "Contoso API",
        "errorUrl": null,
        "logoutUrl": null,
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "samlMetadataUrl": null,
        "microsoftFirstParty": null,
        "publisherName": "f/128 Photography",
        "preferredTokenSigningKeyThumbprint": null,
        "replyUrls": [],
        "servicePrincipalNames": [
            "d7fbfe28-c60e-46d2-8335-841923950d3b"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp",
            "WindowsAzureActiveDirectoryCustomSingleSignOnApplication"
        ],
        "notificationEmailAddresses": [],
        "keyCredentials": [],
        "passwordCredentials": []
    }
}
```


### <a name="retrieve-app-object-id-and-service-principal-object-id"></a><span data-ttu-id="92efe-144">检索应用对象 ID 和服务主体对象 ID</span><span class="sxs-lookup"><span data-stu-id="92efe-144">Retrieve app object ID and service principal object ID</span></span>
<span data-ttu-id="92efe-145">使用上一次调用的响应检索并保存应用程序对象 ID 和服务主体对象 ID。</span><span class="sxs-lookup"><span data-stu-id="92efe-145">Use the response from the previous call to retrieve and save the application object ID and service principal object ID.</span></span>
```
"application": {
    "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83"
    }
"servicePrincipal": {
    "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
    }
```

## <a name="step-2-configure-application-proxy-properties"></a><span data-ttu-id="92efe-146">步骤2：配置应用程序代理属性</span><span class="sxs-lookup"><span data-stu-id="92efe-146">Step 2: Configure Application Proxy properties</span></span>

### <a name="set-the-onpremisespublishing-configuration"></a><span data-ttu-id="92efe-147">设置 onPremisesPublishing 配置</span><span class="sxs-lookup"><span data-stu-id="92efe-147">Set the onPremisesPublishing configuration</span></span>

<span data-ttu-id="92efe-148">使用上一步中的 applicationId 为应用程序配置应用程序代理，并将 **onPremisesPublishing** 属性更新为所需的配置。</span><span class="sxs-lookup"><span data-stu-id="92efe-148">Use the applicationId from the previous step to configure Application Proxy for the app and update the **onPremisesPublishing** property to the desired configuration.</span></span> <span data-ttu-id="92efe-149">在此示例中，您使用的是内部 url 的应用程序： `https://contosoiwaapp.com` 并使用外部 url 的默认域： `https://contosoiwaapp-contoso.msappproxy.net` 。</span><span class="sxs-lookup"><span data-stu-id="92efe-149">In this example, you're using an app with the internal url: `https://contosoiwaapp.com` and using the default domain for the external url: `https://contosoiwaapp-contoso.msappproxy.net`.</span></span> 

#### <a name="request"></a><span data-ttu-id="92efe-150">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="92efe-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="92efe-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92efe-152">C#</span><span class="sxs-lookup"><span data-stu-id="92efe-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92efe-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92efe-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92efe-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92efe-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92efe-155">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="set-the-redirecturi-identifieruri-and-homepageurl-properties"></a><span data-ttu-id="92efe-156">设置 redirectUri、identifierUri 和 homepageUrl 属性</span><span class="sxs-lookup"><span data-stu-id="92efe-156">Set the redirectUri, identifierUri, and homepageUrl properties</span></span>
<span data-ttu-id="92efe-157">将应用程序的 " **redirectUri**"、" **identifierUri**" 和 " **homepageUrl** " propertes 更新为外部 URL。</span><span class="sxs-lookup"><span data-stu-id="92efe-157">Update the application's **redirectUri**, **identifierUri**, and **homepageUrl** propertes to the external URL.</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-158">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-158">Request</span></span>

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
      "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net"
   }
}
```
#### <a name="response"></a><span data-ttu-id="92efe-159">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a><span data-ttu-id="92efe-160">步骤3：将连接器组分配给应用程序</span><span class="sxs-lookup"><span data-stu-id="92efe-160">Step 3: Assign the connector group to the application</span></span>

### <a name="get-connectors"></a><span data-ttu-id="92efe-161">获取连接器</span><span class="sxs-lookup"><span data-stu-id="92efe-161">Get connectors</span></span>

<span data-ttu-id="92efe-162">列出连接器并使用响应来检索和保存连接器对象 ID。</span><span class="sxs-lookup"><span data-stu-id="92efe-162">List the connectors and use the response to retrieve and save the connector object ID.</span></span> <span data-ttu-id="92efe-163">连接器对象 ID 将用于将连接器分配给连接器组。</span><span class="sxs-lookup"><span data-stu-id="92efe-163">The connector object ID will be used to assign the connector to a connector group.</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-164">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="92efe-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="92efe-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[<span data-ttu-id="92efe-166">C#</span><span class="sxs-lookup"><span data-stu-id="92efe-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92efe-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92efe-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92efe-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92efe-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92efe-169">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-169">Response</span></span>

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

### <a name="create-a-connectorgroup"></a><span data-ttu-id="92efe-170">创建 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="92efe-170">Create a connectorGroup</span></span>
<span data-ttu-id="92efe-171">在此示例中，创建了一个用于应用程序的名为 "IWA Demo Connector Group" 的新 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="92efe-171">For this example, a new connectorGroup is created named "IWA Demo Connector Group" that is used for the application.</span></span> <span data-ttu-id="92efe-172">如果您的连接器已分配给相应的 connectorGroup，也可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="92efe-172">You can also skip this step if your connector is already assigned to the appropriate connectorGroup.</span></span> <span data-ttu-id="92efe-173">检索并保存要在下一步中使用的 connectorGroup 对象 ID。</span><span class="sxs-lookup"><span data-stu-id="92efe-173">Retrieve and save the connectorGroup object ID to use in the next step.</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-174">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-174">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="92efe-175">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-175">Response</span></span>

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

### <a name="assign-a-connector-to-the-connectorgroup"></a><span data-ttu-id="92efe-176">将连接器分配给 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="92efe-176">Assign a connector to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-177">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-177">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="92efe-178">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-178">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a><span data-ttu-id="92efe-179">将应用程序分配给 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="92efe-179">Assign the application to the connectorGroup</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-180">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="92efe-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="92efe-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92efe-182">C#</span><span class="sxs-lookup"><span data-stu-id="92efe-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92efe-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92efe-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92efe-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92efe-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="92efe-185">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a><span data-ttu-id="92efe-186">步骤4：配置单一登录</span><span class="sxs-lookup"><span data-stu-id="92efe-186">Step 4: Configure single sign-on</span></span>
<span data-ttu-id="92efe-187">此应用程序使用集成的 Windows 身份验证 (IWA) 。</span><span class="sxs-lookup"><span data-stu-id="92efe-187">This application uses Integrated Windows Authentication (IWA).</span></span> <span data-ttu-id="92efe-188">若要配置 IWA，请在 [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) 资源类型中设置单一登录属性。</span><span class="sxs-lookup"><span data-stu-id="92efe-188">To configure IWA, set the single sign-on properties in the [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) resource type.</span></span>


#### <a name="request"></a><span data-ttu-id="92efe-189">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-189">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="92efe-190">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-190">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a><span data-ttu-id="92efe-191">第 5 步：分配用户</span><span class="sxs-lookup"><span data-stu-id="92efe-191">Step 5: Assign users</span></span>
### <a name="retrieve-approle-for-the-applicaiton"></a><span data-ttu-id="92efe-192">检索应用程序的 appRole</span><span class="sxs-lookup"><span data-stu-id="92efe-192">Retrieve appRole for the applicaiton</span></span>

#### <a name="request"></a><span data-ttu-id="92efe-193">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-193">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="92efe-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="92efe-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoles
```
# <a name="c"></a>[<span data-ttu-id="92efe-195">C#</span><span class="sxs-lookup"><span data-stu-id="92efe-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92efe-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92efe-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92efe-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92efe-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="92efe-198">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-198">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('b00c693f-9658-4c06-bd1b-c402c4653dea')/appRoles",
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

<span data-ttu-id="92efe-199">使用上一次调用中的响应检索并保存 appRole ID 以用于下一步。</span><span class="sxs-lookup"><span data-stu-id="92efe-199">Use the response from the previous call to retrieve and save the appRole ID to use for the next step.</span></span>
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a><span data-ttu-id="92efe-200">向应用程序分配用户和组</span><span class="sxs-lookup"><span data-stu-id="92efe-200">Assign users and groups to the application</span></span>

<span data-ttu-id="92efe-201">使用以下属性将用户分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="92efe-201">Use the following properties to assign a user to the application.</span></span>

| <span data-ttu-id="92efe-202">属性</span><span class="sxs-lookup"><span data-stu-id="92efe-202">Property</span></span>  | <span data-ttu-id="92efe-203">说明</span><span class="sxs-lookup"><span data-stu-id="92efe-203">Description</span></span> |<span data-ttu-id="92efe-204">ID</span><span class="sxs-lookup"><span data-stu-id="92efe-204">ID</span></span>  |
|---------|---------|---------|
| <span data-ttu-id="92efe-205">principalId</span><span class="sxs-lookup"><span data-stu-id="92efe-205">principalId</span></span> | <span data-ttu-id="92efe-206">将分配给应用程序的用户的用户 ID</span><span class="sxs-lookup"><span data-stu-id="92efe-206">User ID of the user that will be assigned to the app</span></span> | <span data-ttu-id="92efe-207">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span><span class="sxs-lookup"><span data-stu-id="92efe-207">2fe96d23-5dc6-4f35-8222-0426a8c115c8</span></span> |
| <span data-ttu-id="92efe-208">principalType</span><span class="sxs-lookup"><span data-stu-id="92efe-208">principalType</span></span> | <span data-ttu-id="92efe-209">用户类型</span><span class="sxs-lookup"><span data-stu-id="92efe-209">Type of user</span></span> | <span data-ttu-id="92efe-210">用户</span><span class="sxs-lookup"><span data-stu-id="92efe-210">User</span></span> |
| <span data-ttu-id="92efe-211">appRoleId</span><span class="sxs-lookup"><span data-stu-id="92efe-211">appRoleId</span></span> |  <span data-ttu-id="92efe-212">应用程序的默认应用程序角色的应用程序角色 ID</span><span class="sxs-lookup"><span data-stu-id="92efe-212">The App role ID of the default app role of the app</span></span> | <span data-ttu-id="92efe-213">18d14569-c3bd-439b-9a66-3a2aee01d14f</span><span class="sxs-lookup"><span data-stu-id="92efe-213">18d14569-c3bd-439b-9a66-3a2aee01d14f</span></span> |
| <span data-ttu-id="92efe-214">resourceId</span><span class="sxs-lookup"><span data-stu-id="92efe-214">resourceId</span></span> | <span data-ttu-id="92efe-215">应用程序的 servicePrincipal ID</span><span class="sxs-lookup"><span data-stu-id="92efe-215">The servicePrincipal ID of the app</span></span> | <span data-ttu-id="92efe-216">b00c693f-9658-4c06-bd1b-c402c4653dea</span><span class="sxs-lookup"><span data-stu-id="92efe-216">b00c693f-9658-4c06-bd1b-c402c4653dea</span></span> |

#### <a name="request"></a><span data-ttu-id="92efe-217">请求</span><span class="sxs-lookup"><span data-stu-id="92efe-217">Request</span></span>


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
  "resourceId":"b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```

#### <a name="response"></a><span data-ttu-id="92efe-218">响应</span><span class="sxs-lookup"><span data-stu-id="92efe-218">Response</span></span>

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
    "resourceId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```

<span data-ttu-id="92efe-219">有关详细信息，请参阅 [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="92efe-219">For more information, see [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) resource type.</span></span>



## <a name="additional-steps"></a><span data-ttu-id="92efe-220">其他步骤</span><span class="sxs-lookup"><span data-stu-id="92efe-220">Additional steps</span></span>
- [<span data-ttu-id="92efe-221">使用 PowerShell 示例为应用程序代理自动执行配置</span><span class="sxs-lookup"><span data-stu-id="92efe-221">Automate configuration using PowerShell samples for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [<span data-ttu-id="92efe-222">使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置</span><span class="sxs-lookup"><span data-stu-id="92efe-222">Automate SAML-based SSO app configuration with Microsoft Graph API</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
