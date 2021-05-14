---
title: 使用 Microsoft Graph API 配置基于 SAML 的单一登录
description: 了解如何通过使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录来节省时间。
author: kenwith
localization_priority: Priority
ms.custom: scenarios:getting-started
ms.prod: applications
ms.openlocfilehash: 16382da1b71e36de93dcffb0e8ebb048c5460f5e
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335692"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a><span data-ttu-id="5a60c-103">使用 Microsoft Graph API 为应用程序配置基于 SAML 的单一登录</span><span class="sxs-lookup"><span data-stu-id="5a60c-103">Configure SAML-based single sign-on for your application using the Microsoft Graph API</span></span>

<span data-ttu-id="5a60c-104">本文介绍了如何使用 Microsoft Graph API 为 Azure Active Directory （Azure AD） 中的应用程序创建和配置基于 SAML 的单一登录 （SSO）。</span><span class="sxs-lookup"><span data-stu-id="5a60c-104">In this article, you'll learn how to create and configure a SAML-based single sign-on (SSO) for your application in Azure Active Directory (Azure AD) using the Microsoft Graph API.</span></span> <span data-ttu-id="5a60c-105">应用程序配置包括基本 SAML URL、声明映射策略以及使用证书添加自定义签名密钥。</span><span class="sxs-lookup"><span data-stu-id="5a60c-105">The application configuration includes basic SAML URLs, a claims mapping policy, and using a certificate to add a custom signing key.</span></span> <span data-ttu-id="5a60c-106">创建应用程序后，可以为其分配管理员用户。</span><span class="sxs-lookup"><span data-stu-id="5a60c-106">After the application is created, you assign a user to it to be an administrator.</span></span> <span data-ttu-id="5a60c-107">然后，可以使用 URL 获取 Azure AD SAML 元数据，以对应用程序进行其他配置。</span><span class="sxs-lookup"><span data-stu-id="5a60c-107">You then can use a URL to obtain Azure AD SAML metadata for additional configuration of the application.</span></span> 

<span data-ttu-id="5a60c-108">本文使用 AWS Azure AD 应用程序模板作为示例，但可以针对 Azure AD 库中的任何基于 SAML 的应用使用本文中的步骤。</span><span class="sxs-lookup"><span data-stu-id="5a60c-108">This article uses an AWS Azure AD application template as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

>[!NOTE]
><span data-ttu-id="5a60c-109">本文中所示的响应对象和密钥可能会被缩短以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="5a60c-109">The response objects and keys shown in this article might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a60c-110">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a60c-110">Prerequisites</span></span>

<span data-ttu-id="5a60c-111">本教程的前提是使用 Microsoft Graph Explorer，但是可以使用 Postman，也可以创建自己的客户端应用程序来调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="5a60c-111">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="5a60c-112">如果要在本教程中调用 Microsoft Graph API，需要使用具有全局管理员角色和适当权限的帐户。</span><span class="sxs-lookup"><span data-stu-id="5a60c-112">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="5a60c-113">对于本教程，需要`Application.ReadWrite.All`、`AppRoleAssignment.ReadWrite.All`、`Policy.Read.All`、`Policy.ReadWrite.ApplicationConfiguration` 和 `User.ReadWrite.All` 委派权限。</span><span class="sxs-lookup"><span data-stu-id="5a60c-113">For this tutorial, the `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All`, `Policy.ReadWrite.ApplicationConfiguration`, and `User.ReadWrite.All` delegated permissions are needed.</span></span> <span data-ttu-id="5a60c-114">完成以下步骤以在 Microsoft Graph 浏览器中设置权限：</span><span class="sxs-lookup"><span data-stu-id="5a60c-114">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>

1. <span data-ttu-id="5a60c-115">转到 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="5a60c-115">Go to [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
2. <span data-ttu-id="5a60c-116">选择“**使用 Microsoft 登录**”，然后使用 Azure AD 全局管理员账户登录。</span><span class="sxs-lookup"><span data-stu-id="5a60c-116">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="5a60c-117">成功登录后，可在左侧窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="5a60c-117">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
3. <span data-ttu-id="5a60c-118">选择用户帐户详细信息右侧的设置图标，然后选择“**权限**”。</span><span class="sxs-lookup"><span data-stu-id="5a60c-118">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

    ![选择 Microsoft Graph 权限](./images/application-saml-sso-configure-api/set-permissions.png)
        
4. <span data-ttu-id="5a60c-120">在权限列表中，滚动到并展开“**AppRoleAssignment (1)**”，然后选择“**AppRoleAssignment.ReadWrite.All**”权限。</span><span class="sxs-lookup"><span data-stu-id="5a60c-120">In the list of permissions, scroll to and expand **AppRoleAssignment (1)**, and then select the **AppRoleAssignment.ReadWrite.All** permission.</span></span> <span data-ttu-id="5a60c-121">继续向下滚动并展开“**应用程序 (2)**”，然后选择“**Application.ReadWrite.All**”权限。</span><span class="sxs-lookup"><span data-stu-id="5a60c-121">Scroll further down and expand **Application (2)**, and then select the **Application.ReadWrite.All** permission.</span></span> <span data-ttu-id="5a60c-122">继续滚动到并选择“**策略 (13)**”，然后选择“**Policy.Read.All**”和“**Policy.ReadWrite.ApplicationConfiguration**”权限。</span><span class="sxs-lookup"><span data-stu-id="5a60c-122">Continue to and expand **Policy (13)**, and then select the **Policy.Read.All**  and **Policy.ReadWrite.ApplicationConfiguration** permissions.</span></span> <span data-ttu-id="5a60c-123">最后，滚动到并展开“**用户 (8)**”，然后选择“**User.ReadWrite.All**”。</span><span class="sxs-lookup"><span data-stu-id="5a60c-123">Finally, scroll to and expand **Users (8)**, and then select **User.ReadWrite.All**.</span></span> 

    ![滚动并选择 approleasignment、应用程序和策略权限](./images/application-saml-sso-configure-api/select-permissions.png)

5. <span data-ttu-id="5a60c-125">选择“**同意**”，然后选择“**接受**”，以接受同意权限。</span><span class="sxs-lookup"><span data-stu-id="5a60c-125">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="5a60c-126">你不需要代表组织同意这些权限。</span><span class="sxs-lookup"><span data-stu-id="5a60c-126">You do not need to consent on behalf of your organization for these permissions.</span></span>

    ![接受同意权限](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a><span data-ttu-id="5a60c-128">第 1 步：创建应用程序</span><span class="sxs-lookup"><span data-stu-id="5a60c-128">Step 1: Create the application</span></span>

<span data-ttu-id="5a60c-129">Azure AD 中存在一个库，其中包含数千个预集成的应用程序，可以将其用作应用程序的模板。</span><span class="sxs-lookup"><span data-stu-id="5a60c-129">Azure AD has a gallery that contains thousands of pre-integrated applications that you can use as a template for your application.</span></span> <span data-ttu-id="5a60c-130">应用程序模板描述了该应用程序的元数据。</span><span class="sxs-lookup"><span data-stu-id="5a60c-130">The application template describes the metadata for that application.</span></span> <span data-ttu-id="5a60c-131">使用此模板，可以在租户中创建应用程序和服务主体的实例以进行管理。</span><span class="sxs-lookup"><span data-stu-id="5a60c-131">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span> 

<span data-ttu-id="5a60c-132">如果要从库中创建应用程序，首先获取应用程序模板的标识符，然后使用该标识符创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="5a60c-132">To create the application from the gallery, you first get the identifier of the application template and then use that identifier to create the application.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="5a60c-133">检索库应用程序模板标识符</span><span class="sxs-lookup"><span data-stu-id="5a60c-133">Retrieve the gallery application template identifier</span></span>

 <span data-ttu-id="5a60c-134">在本教程中，将检索 `AWS Single Sign-on` 应用程序模板的标识符。</span><span class="sxs-lookup"><span data-stu-id="5a60c-134">In this tutorial, you retrieve the identifier of the application template for `AWS Single Sign-on`.</span></span> <span data-ttu-id="5a60c-135">记录 **id** 属性值，以供稍后在本教程中使用。</span><span class="sxs-lookup"><span data-stu-id="5a60c-135">Record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-136">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-136">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/applicationTemplates?$filter=displayName eq 'AWS Single Sign-on'
```

#### <a name="response"></a><span data-ttu-id="5a60c-137">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-137">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applicationTemplates",
  "value": [
    {
      "id": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
      "displayName": "AWS Single Sign-on",
      "homePageUrl": "https://aws.amazon.com/",
      "supportedSingleSignOnModes": [
        "saml",
        "external"
      ],
      "supportedProvisioningTypes": [
        "sync"
      ],
      "logoUrl": "https://az495088.vo.msecnd.net/app-logo/awssinglesignon_215.png",
      "categories": [
        "developerServices",
        "itInfrastructure",
        "security",
        "New"
      ],
      "publisher": "Amazon Web Services, Inc.",
      "description": "Federate once to AWS SSO & use it to manage access centrally to multiple AWS accounts. Provision users via SCIM & get Azure AD single sign-in access to the AWS Console, CLI, & AWS SSO integrated apps."
    }
  ]
}
```

### <a name="create-the-application"></a><span data-ttu-id="5a60c-138">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="5a60c-138">Create the application</span></span>

<span data-ttu-id="5a60c-139">使用为应用模板记录的 **id** 值，在租户中为应用和服务主题创建实例。</span><span class="sxs-lookup"><span data-stu-id="5a60c-139">Using the **id** value that you recorded for the application template, create an instance of the application and service principal in your tenant.</span></span> <span data-ttu-id="5a60c-140">记录应用程序的 **id** 属性值和服务主体的 **id** 属性值，以在本教程中稍后使用。</span><span class="sxs-lookup"><span data-stu-id="5a60c-140">Record the value of the **id** property of the application and the value of the **id** property for the service principal to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-141">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-141">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/21ed01d2-ec13-4e9e-86c1-cd546719ebc4/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> <span data-ttu-id="5a60c-142">留出一些时间将应用程序配置到 Azure AD 租户中。</span><span class="sxs-lookup"><span data-stu-id="5a60c-142">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="5a60c-143">这不是即时的。</span><span class="sxs-lookup"><span data-stu-id="5a60c-143">It is not instant.</span></span> <span data-ttu-id="5a60c-144">一种策略是每 5-10秒 对应用程序或服务主体对象执行 GET 查询，直到查询成功。</span><span class="sxs-lookup"><span data-stu-id="5a60c-144">One strategy is to do a GET query on the application or service principal object every 5-10 seconds until the query is successful.</span></span>

#### <a name="response"></a><span data-ttu-id="5a60c-145">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-145">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "id": "a9be408a-6c31-4141-8cea-52fcd4a61be8",
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "createdDateTime": "2021-05-10T20:12:03Z",
    "deletedDateTime": null,
    "displayName": "AWS Contoso",
    "groupMembershipClaims": null,
    "identifierUris": [],
    "isFallbackPublicClient": false,
    "signInAudience": "AzureADMyOrg",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "defaultRedirectUri": null,
    "optionalClaims": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "api": {
      "acceptMappedClaims": null,
      "knownClientApplications": [],
      "requestedAccessTokenVersion": null,
      "oauth2PermissionScopes": [
        {
          "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
          "adminConsentDisplayName": "Access AWS Contoso",
          "id": "6f891cd3-c132-4822-930b-f343b4515d19",
          "isEnabled": true,
          "type": "User",
          "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
          "userConsentDisplayName": "Access AWS Contoso",
          "value": "user_impersonation"
        }
      ],
      "preAuthorizedApplications": []
    },
    "appRoles": [
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
        "isEnabled": true,
        "description": "msiam_access",
        "value": null,
        "origin": "Application"
      }
    ],
    "info": {
      "logoUrl": null,
      "marketingUrl": null,
      "privacyStatementUrl": null,
      "supportUrl": null,
      "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
      "countriesBlockedForMinors": [],
      "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "publicClient": {
      "redirectUris": []
    },
    "requiredResourceAccess": [],
    "web": {
      "homePageUrl": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
      "redirectUris": []
    }
  },
  "servicePrincipal": {
    "id": "a750f6cf-2319-464a-bcc3-456926736a91",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "appDisplayName": "AWS Contoso",
    "alternativeNames": [],
    "appOwnerOrganizationId": "8500cad3-193d-48a6-8d00-c129b114dc10",
    "displayName": "AWS Contoso",
    "appRoleAssignmentRequired": true,
    "loginUrl": null,
    "logoutUrl": null,
    "homepage": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
    "notificationEmailAddresses": [],
    "preferredSingleSignOnMode": null,
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [],
    "servicePrincipalNames": [
      "17cad0e7-cd2b-4e51-a75d-ba810f3e4045"
    ],
    "servicePrincipalType": "Application",
    "tags": [
      "WindowsAzureActiveDirectoryIntegratedApp"
    ],
    "tokenEncryptionKeyId": null,
    "samlSingleSignOnSettings": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "appRoles": [
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
        "isEnabled": true,
        "description": "msiam_access",
        "value": null,
        "origin": "Application"
      }
    ],
    "info": {
      "logoUrl": null,
      "marketingUrl": null,
      "privacyStatementUrl": null,
      "supportUrl": null,
      "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [
      {
        "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
        "adminConsentDisplayName": "Access AWS Contoso",
        "id": "6f891cd3-c132-4822-930b-f343b4515d19",
        "isEnabled": true,
        "type": "User",
        "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
        "userConsentDisplayName": "Access AWS Contoso",
        "value": "user_impersonation"
      }
    ],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="5a60c-146">第 2 步：配置单一登录</span><span class="sxs-lookup"><span data-stu-id="5a60c-146">Step 2: Configure single sign-on</span></span>

<span data-ttu-id="5a60c-147">在本教程中，`saml`设置为服务主体中的单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="5a60c-147">In this tutorial, you set `saml` as the single sign-on mode in the service principal.</span></span> <span data-ttu-id="5a60c-148">使用之前记录的服务主体 **id**。</span><span class="sxs-lookup"><span data-stu-id="5a60c-148">Use the **id** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-149">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-149">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-150">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-150">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a><span data-ttu-id="5a60c-151">设置基本 SAML URL</span><span class="sxs-lookup"><span data-stu-id="5a60c-151">Set basic SAML URLs</span></span>

<span data-ttu-id="5a60c-152">使用之前记录的应用程序 **id**，设置标识符 URI，并在应用程序对象中重定向 AWS 的 URI。</span><span class="sxs-lookup"><span data-stu-id="5a60c-152">Using the **id** for the application that you recorded earlier, set the identifier URI and redirect URI for AWS in the application object.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-153">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-153">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
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

#### <a name="response"></a><span data-ttu-id="5a60c-154">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-154">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a><span data-ttu-id="5a60c-155">添加应用程序角色（可选）</span><span class="sxs-lookup"><span data-stu-id="5a60c-155">Add app roles (Optional)</span></span>

<span data-ttu-id="5a60c-156">如果应用程序需要令牌中的角色信息，请在应用程序对象中添加角色的定义。</span><span class="sxs-lookup"><span data-stu-id="5a60c-156">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> 

> [!NOTE] 
> <span data-ttu-id="5a60c-157">添加应用程序角色时，请勿修改默认应用程序角色 `msiam_access`。</span><span class="sxs-lookup"><span data-stu-id="5a60c-157">When adding app roles, don't modify the default app roles `msiam_access`.</span></span> 

<span data-ttu-id="5a60c-158">使用之前记录的服务主体 **id**。</span><span class="sxs-lookup"><span data-stu-id="5a60c-158">Use the **id** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-159">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-159">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/a9be408a-6c31-4141-8cea-52fcd4a61be8
Content-type: serviceprincipals/json

{
  "appRoles": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "User",
      "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
      "isEnabled": true,
      "description": "User",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "msiam_access",
      "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
      "isEnabled": true,
      "description": "msiam_access",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Admin,WAAD",
      "displayName": "Admin,WAAD",
      "id": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Finance,WAAD",
      "displayName": "Finance,WAAD",
      "id": "7a960000-ded3-455b-8c04-4f2ace00319b",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-160">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-160">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="5a60c-161">第 3 步：配置声明映射</span><span class="sxs-lookup"><span data-stu-id="5a60c-161">Step 3: Configure claims mapping</span></span>

### <a name="create-a-claims-mapping-policy"></a><span data-ttu-id="5a60c-162">创建声明映射策略</span><span class="sxs-lookup"><span data-stu-id="5a60c-162">Create a claims mapping policy</span></span>

<span data-ttu-id="5a60c-163">除了基本声明之外，还为 Azure AD 配置以下声明以在 SAML 令牌中发出：</span><span class="sxs-lookup"><span data-stu-id="5a60c-163">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="5a60c-164">声明名称</span><span class="sxs-lookup"><span data-stu-id="5a60c-164">Claim name</span></span> | <span data-ttu-id="5a60c-165">源</span><span class="sxs-lookup"><span data-stu-id="5a60c-165">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="5a60c-166">assignedroles</span><span class="sxs-lookup"><span data-stu-id="5a60c-166">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="5a60c-167">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="5a60c-167">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="5a60c-168">"900"</span><span class="sxs-lookup"><span data-stu-id="5a60c-168">"900"</span></span> |
| <span data-ttu-id="5a60c-169">roles</span><span class="sxs-lookup"><span data-stu-id="5a60c-169">roles</span></span> | <span data-ttu-id="5a60c-170">assignedroles</span><span class="sxs-lookup"><span data-stu-id="5a60c-170">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="5a60c-171">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="5a60c-171">userprincipalname</span></span> |

> [!NOTE]
> <span data-ttu-id="5a60c-172">声明映射策略中的某些项区分大小写（例如“Version”）。</span><span class="sxs-lookup"><span data-stu-id="5a60c-172">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="5a60c-173">如果收到错误消息，例如“属性的值无效”，则可能是区分大小写的问题。</span><span class="sxs-lookup"><span data-stu-id="5a60c-173">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

<span data-ttu-id="5a60c-174">创建声明映射策略并创建 **id**，以随后在本教程中使用。</span><span class="sxs-lookup"><span data-stu-id="5a60c-174">Create the claims mapping policy and record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-175">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-175">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-176">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-176">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: claimsMappingPolicies/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
  "id": "a4b35718-fd5e-4ca8-8248-a3c9934b1b78",
  "deletedDateTime": null,
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
  ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a><span data-ttu-id="5a60c-177">向服务主体分配声明映射策略</span><span class="sxs-lookup"><span data-stu-id="5a60c-177">Assign a claims mapping policy to a service principal</span></span>

<span data-ttu-id="5a60c-178">使用之前记录的服务主体 **id** 为其分配映射策略。</span><span class="sxs-lookup"><span data-stu-id="5a60c-178">Use the **id** for the service principal that you recorded earlier to assign a claims mapping policy to it.</span></span> <span data-ttu-id="5a60c-179">将 **id** 属性值用于请求正文中的声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="5a60c-179">Use the value of the **id** property for the claims mapping policy in the body of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-180">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-180">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78"
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-181">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-181">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a><span data-ttu-id="5a60c-182">第 4 步：配置签名证书</span><span class="sxs-lookup"><span data-stu-id="5a60c-182">Step 4: Configure a signing certificate</span></span>

<span data-ttu-id="5a60c-183">你需要一个自签名证书，Azure AD 可以使用该证书来签署 SAML 响应。</span><span class="sxs-lookup"><span data-stu-id="5a60c-183">You need a self-signed certificate that Azure AD can use to sign a SAML response.</span></span> <span data-ttu-id="5a60c-184">可以使用自己的证书，也可以使用以下示例。</span><span class="sxs-lookup"><span data-stu-id="5a60c-184">You can use your own certificate or you can use the following example.</span></span> 

### <a name="create-a-signing-certificate"></a><span data-ttu-id="5a60c-185">创建签名证书</span><span class="sxs-lookup"><span data-stu-id="5a60c-185">Create a signing certificate</span></span>

<span data-ttu-id="5a60c-186">使用所创建的服务主体 **id**，创建新的证书并将其添加到服务主体。</span><span class="sxs-lookup"><span data-stu-id="5a60c-186">Using the **id** of the service principal that you created, create a new certificate and add it to the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-187">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-187">Request</span></span>

```http
POST https://graph.microsoft.com/beta/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=AWSContoso",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-188">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-188">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "p9PEYmuKhP2oaMzGfSdNQC/9ChA=",
  "displayName": "CN=AWSContoso",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICqjCCAZKgAwIBAgIId....4rnrk43wp75yqjRbOhAZ1ExAxVqW+o2JslhjUeltUMNQW+ynOfs9oHu1ZdnGmxrE=",
  "keyId": "70883316-50be-4016-ba80-19d9fbad873d",
  "startDateTime": "2021-05-10T20:35:37.5754318Z",
  "thumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="5a60c-189">激活自定义签名密钥</span><span class="sxs-lookup"><span data-stu-id="5a60c-189">Activate the custom signing key</span></span>

<span data-ttu-id="5a60c-190">需要将服务主体的 **preferredTokenSigningKeyThumbprint** 属性设置为想要Azure AD 用于签署 SAML 响应的证书指纹。</span><span class="sxs-lookup"><span data-stu-id="5a60c-190">You need to set the **preferredTokenSigningKeyThumbprint** property of the service principal to the thumbprint of the certificate that you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="5a60c-191">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-191">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: servicePrincipals/json

{
  "preferredTokenSigningKeyThumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10"
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-192">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-192">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a><span data-ttu-id="5a60c-193">第 5 步：分配用户</span><span class="sxs-lookup"><span data-stu-id="5a60c-193">Step 5: Assign users</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="5a60c-194">创建用户账户</span><span class="sxs-lookup"><span data-stu-id="5a60c-194">Create a user account</span></span>

<span data-ttu-id="5a60c-195">对于本教程，将创建一个添加到应用程序中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="5a60c-195">For this tutorial, you create a user account that is added to the application.</span></span> <span data-ttu-id="5a60c-196">在请求正文中，将 contoso.com 更改为租户的域名。</span><span class="sxs-lookup"><span data-stu-id="5a60c-196">In the request body, change contoso.com to the domain name of your tenant.</span></span> <span data-ttu-id="5a60c-197">可在 Azure Active Directory 概述页面上找到租户信息。</span><span class="sxs-lookup"><span data-stu-id="5a60c-197">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="5a60c-198">记录要在本教程后面要使用的用户 **id**。</span><span class="sxs-lookup"><span data-stu-id="5a60c-198">Record the **id** of the user to be used later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-199">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-199">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-200">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-200">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

### <a name="assign-a-user-to-the-application"></a><span data-ttu-id="5a60c-201">向应用程序分配用户</span><span class="sxs-lookup"><span data-stu-id="5a60c-201">Assign a user to the application</span></span>

<span data-ttu-id="5a60c-202">将创建的用户分配给服务主体，然后分配 `Admin,WAAD` 应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="5a60c-202">Assign the user that you created to the service principal and assign the `Admin,WAAD` app role.</span></span> 

<span data-ttu-id="5a60c-203">在请求正文中，提供这些值：</span><span class="sxs-lookup"><span data-stu-id="5a60c-203">In the request body, provide these values:</span></span>

- <span data-ttu-id="5a60c-204">**principalId** - 所创建的用户账户的 **id**。</span><span class="sxs-lookup"><span data-stu-id="5a60c-204">**principalId** - The **id** of the user account that you created.</span></span>
- <span data-ttu-id="5a60c-205">**appRoleId** - 新增 `Admin,WAAD` 应用程序角色的 **id**。</span><span class="sxs-lookup"><span data-stu-id="5a60c-205">**appRoleId** - The **id** of the `Admin,WAAD` app role that you added.</span></span>
- <span data-ttu-id="5a60c-206">**resourceId** - 服务主体的 **id**。</span><span class="sxs-lookup"><span data-stu-id="5a60c-206">**resourceId** - The **id** of the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-207">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-207">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "appRoleId":"3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "resourceId":"a750f6cf-2319-464a-bcc3-456926736a91"
}
```

#### <a name="response"></a><span data-ttu-id="5a60c-208">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-208">Response</span></span>

```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('a750f6cf-2319-464a-bcc3-456926736a91')/appRoleAssignments/$entity",
  "id": "mZUPBA98lE-qdYOUxMbqm2qY3odGRGdFtpYJkAfUC0Q",
  "deletedDateTime": null,
  "appRoleId": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "createdDateTime": "2021-05-10T21:04:11.0480851Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "a750f6cf-2319-464a-bcc3-456926736a91"
}
```

## <a name="step-6-get-azure-ad-saml-metadata"></a><span data-ttu-id="5a60c-209">第 6 步：获取 Azure AD SAML 元数据</span><span class="sxs-lookup"><span data-stu-id="5a60c-209">Step 6: Get Azure AD SAML metadata</span></span>

<span data-ttu-id="5a60c-210">使用以下 URL 获取特定配置的应用程序的 Azure AD SAML 元数据。</span><span class="sxs-lookup"><span data-stu-id="5a60c-210">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="5a60c-211">元数据包含诸如签名证书、Azure AD entityID和 Azure AD SingleSignOnService 等信息。</span><span class="sxs-lookup"><span data-stu-id="5a60c-211">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

<span data-ttu-id="5a60c-212">下面显示了可能在应用程序中看到的示例：</span><span class="sxs-lookup"><span data-stu-id="5a60c-212">The following shows an example of what you might see for your application:</span></span>

```
<EntityDescriptor xmlns="urn:oasis:names:tc:SAML:2.0:metadata" ID="_05fbbf53-e892-43c9-9300-1f6738ace02c" entityID="https://sts.windows.net/2f82f566-5953-43f4-9251-79c6009bdf24/">
<Signature xmlns="http://www.w3.org/2000/09/xmldsig#">

...

<SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
</IDPSSODescriptor>
</EntityDescriptor>
```

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="5a60c-213">第 7 步：清理资源</span><span class="sxs-lookup"><span data-stu-id="5a60c-213">Step 7: Clean up resources</span></span>

<span data-ttu-id="5a60c-214">在此步骤中，将删除创建的资源。</span><span class="sxs-lookup"><span data-stu-id="5a60c-214">In this step, you remove the resources that you created.</span></span>


### <a name="delete-the-application"></a><span data-ttu-id="5a60c-215">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="5a60c-215">Delete the application</span></span>

<span data-ttu-id="5a60c-216">删除创建的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5a60c-216">Delete the application that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-217">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-217">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
```

#### <a name="response"></a><span data-ttu-id="5a60c-218">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-218">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="5a60c-219">删除用户账户</span><span class="sxs-lookup"><span data-stu-id="5a60c-219">Delete the user account</span></span>

<span data-ttu-id="5a60c-220">删除 MyTestUser1 用户帐户。</span><span class="sxs-lookup"><span data-stu-id="5a60c-220">Delete the MyTestUser1 user account.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-221">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-221">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/040f9599-7c0f-4f94-aa75-8394c4c6ea9b
```

#### <a name="response"></a><span data-ttu-id="5a60c-222">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-222">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a><span data-ttu-id="5a60c-223">删除声明映射策略</span><span class="sxs-lookup"><span data-stu-id="5a60c-223">Delete the claims mapping policy</span></span>

<span data-ttu-id="5a60c-224">删除声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="5a60c-224">Delete the claims mapping policy.</span></span>

#### <a name="request"></a><span data-ttu-id="5a60c-225">请求</span><span class="sxs-lookup"><span data-stu-id="5a60c-225">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78
```

#### <a name="response"></a><span data-ttu-id="5a60c-226">响应</span><span class="sxs-lookup"><span data-stu-id="5a60c-226">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="5a60c-227">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5a60c-227">See also</span></span>

- <span data-ttu-id="5a60c-228">对于 AWS，可以[启用用户配置](/azure/active-directory/app-provisioning/application-provisioning-configure-api)以从该 AWS 账户获取所有角色。</span><span class="sxs-lookup"><span data-stu-id="5a60c-228">For AWS, you can [enable user provisioning](/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> <span data-ttu-id="5a60c-229">有关详细信息，请参阅[配置 SAML 令牌中颁发的角色声明](/azure/active-directory/develop/active-directory-enterprise-app-role-management)。</span><span class="sxs-lookup"><span data-stu-id="5a60c-229">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>
- <span data-ttu-id="5a60c-230">[自定义在租户具体应用的令牌中颁发的声明](/azure/active-directory/develop/active-directory-claims-mapping)。</span><span class="sxs-lookup"><span data-stu-id="5a60c-230">[Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
- <span data-ttu-id="5a60c-231">可以使用 applicationTemplate API 来实例化[非库应用程序](/azure/active-directory/manage-apps/view-applications-portal)。</span><span class="sxs-lookup"><span data-stu-id="5a60c-231">You can use the applicationTemplate API to instantiate [Non-Gallery apps](/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="5a60c-232">使用 applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`。</span><span class="sxs-lookup"><span data-stu-id="5a60c-232">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>
- [<span data-ttu-id="5a60c-233">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="5a60c-233">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
- [<span data-ttu-id="5a60c-234">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a60c-234">appRoleAssignment</span></span>](/graph/api/resources/approleassignment?view=graph-rest-1.0)
- [<span data-ttu-id="5a60c-235">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="5a60c-235">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [<span data-ttu-id="5a60c-236">application</span><span class="sxs-lookup"><span data-stu-id="5a60c-236">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
- [<span data-ttu-id="5a60c-237">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="5a60c-237">claimsMappingPolicy</span></span>](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0)
- [<span data-ttu-id="5a60c-238">keyCredential</span><span class="sxs-lookup"><span data-stu-id="5a60c-238">keyCredential</span></span>](/graph/api/resources/keycredential?view=graph-rest-1.0)
- [<span data-ttu-id="5a60c-239">addTokenSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="5a60c-239">addTokenSigningCertificate</span></span>](/graph/api/serviceprincipal-addtokensigningcertificate?view=graph-rest-beta)
