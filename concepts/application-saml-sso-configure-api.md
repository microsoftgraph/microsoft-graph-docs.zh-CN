---
title: 使用 Microsoft Graph API 配置基于 SAML 的单一登录
description: 了解如何通过使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录来节省时间。
author: kenwith
localization_priority: Priority
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: ea4a0a23b19b0b7a7250966f59e3a92e94a40618
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761470"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a><span data-ttu-id="84a50-103">使用 Microsoft Graph API 为应用程序配置基于 SAML 的单一登录</span><span class="sxs-lookup"><span data-stu-id="84a50-103">Configure SAML-based single sign-on for your application using the Microsoft Graph API</span></span>

<span data-ttu-id="84a50-104">本文介绍了如何使用 Microsoft Graph API 为 Azure Active Directory （Azure AD） 中的应用程序创建和配置基于 SAML 的单一登录 （SSO）。</span><span class="sxs-lookup"><span data-stu-id="84a50-104">In this article, you'll learn how to create and configure a SAML-based single sign-on (SSO) for your application in Azure Active Directory (Azure AD) using the Microsoft Graph API.</span></span> <span data-ttu-id="84a50-105">应用程序配置包括基本 SAML URL、声明映射策略以及使用证书添加自定义签名密钥。</span><span class="sxs-lookup"><span data-stu-id="84a50-105">The application configuration includes basic SAML URLs, a claims mapping policy, and using a certificate to add a custom signing key.</span></span> <span data-ttu-id="84a50-106">创建应用程序后，可以为其分配管理员用户。</span><span class="sxs-lookup"><span data-stu-id="84a50-106">After the application is created, you assign a user to it to be an administrator.</span></span> <span data-ttu-id="84a50-107">然后，可以使用 URL 获取 Azure AD SAML 元数据，以对应用程序进行其他配置。</span><span class="sxs-lookup"><span data-stu-id="84a50-107">You then can use a URL to obtain Azure AD SAML metadata for additional configuration of the application.</span></span> 

<span data-ttu-id="84a50-108">本文使用 AWS Azure AD 应用程序模板作为示例，但可以针对 Azure AD 库中的任何基于 SAML 的应用使用本文中的步骤。</span><span class="sxs-lookup"><span data-stu-id="84a50-108">This article uses an AWS Azure AD application template as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

>[!NOTE]
><span data-ttu-id="84a50-109">本文中所示的响应对象和密钥可能会被缩短以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="84a50-109">The response objects and keys shown in this article might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84a50-110">先决条件</span><span class="sxs-lookup"><span data-stu-id="84a50-110">Prerequisites</span></span>

- <span data-ttu-id="84a50-111">在本教程中，需要一个自签名证书，Azure AD 可以使用该证书来签署 SAML 响应。</span><span class="sxs-lookup"><span data-stu-id="84a50-111">In this tutorial, you need a self-signed certificate that Azure AD can use to sign a SAML response.</span></span> <span data-ttu-id="84a50-112">可以使用自有证书，也可以使用类似以下 C# 代码创建测试证书：</span><span class="sxs-lookup"><span data-stu-id="84a50-112">You can use your own certificate or you could use something like the following C# code to create a test certificate:</span></span>

    > <span data-ttu-id="84a50-113">**注意** 该代码 **仅** 用于学习和参考，不应在生产中直接使用。</span><span class="sxs-lookup"><span data-stu-id="84a50-113">**Note** This code is for learning and reference **ONLY** and should not be used as-is in production.</span></span>

    ```C#
    using System;
    using System.Security.Cryptography;
    using System.Security.Cryptography.X509Certificates;
    using System.Text;

    /* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
     * This code uses a self-signed certificate and should not be used 
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
          Console.WriteLine("startDateTime: " + startDate.ToString("o"));

          // Print out the end date in ISO 8601 format.
          DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
          Console.WriteLine("endDateTime: " + endDate.ToString("o"));

          // Print the GUID used for keyId
          string signAndPasswordGuid = Guid.NewGuid().ToString();
          string verifyGuid = Guid.NewGuid().ToString();
          Console.WriteLine("keyId GUID for Sign and passwordCredentials: " + signAndPasswordGuid);
          Console.WriteLine("keyId GUID for Verify: " + verifyGuid);

          // Print out the password.
          Console.WriteLine("Password: {0}", password);

          // Print out a displayName to use as an example.
          Console.WriteLine("displayName: CN=Example");
          Console.WriteLine();

          // Print out the public key.
          Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
          Console.WriteLine();

          // Generate the customKeyIdentifier using hash of thumbprint.
          Console.WriteLine("Cert thumprint: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
          Console.WriteLine("customKeyIdentifier:");
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

            request.CertificateExtensions.Add (
              new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false)
            );

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

    <span data-ttu-id="84a50-114">如果要完成本教程，需要记录证书中的以下值：</span><span class="sxs-lookup"><span data-stu-id="84a50-114">To complete this tutorial you need to record the following values from your certificate:</span></span>

    - <span data-ttu-id="84a50-115">私钥</span><span class="sxs-lookup"><span data-stu-id="84a50-115">Private Key</span></span>
    - <span data-ttu-id="84a50-116">开始日期和时间</span><span class="sxs-lookup"><span data-stu-id="84a50-116">Start date and time</span></span>
    - <span data-ttu-id="84a50-117">结束日期和时间</span><span class="sxs-lookup"><span data-stu-id="84a50-117">End date and time</span></span>
    - <span data-ttu-id="84a50-118">证书密码</span><span class="sxs-lookup"><span data-stu-id="84a50-118">Certificate password</span></span>
    - <span data-ttu-id="84a50-119">显示名称</span><span class="sxs-lookup"><span data-stu-id="84a50-119">Display name</span></span>
    - <span data-ttu-id="84a50-120">公钥</span><span class="sxs-lookup"><span data-stu-id="84a50-120">Public key</span></span>
    - <span data-ttu-id="84a50-121">指纹哈希</span><span class="sxs-lookup"><span data-stu-id="84a50-121">Hash of the thumbprint</span></span>
    - <span data-ttu-id="84a50-122">密钥标识符</span><span class="sxs-lookup"><span data-stu-id="84a50-122">Key identifier</span></span>

    <span data-ttu-id="84a50-123">除了证书值之外，还需要两个所使用 keyId 的新 GUID。</span><span class="sxs-lookup"><span data-stu-id="84a50-123">In addition to the certificate values, you also need two new GUIDS for the keyIds that are used.</span></span> <span data-ttu-id="84a50-124">以下示例显示了之前列出代码的输出：</span><span class="sxs-lookup"><span data-stu-id="84a50-124">The following example shows the output of the previously listed code:</span></span>

    ```
    Private Key: MIIKW...AIBAzTVKCAgfQ

    startDateTime: 2020-12-17T20:33:07.0000000Z
    endDateTime: 2022-12-17T20:33:07.0000000Z
    keyId GUID for Sign and passwordCredentials: ed4f28e8-a502-4440-bfba-6038cb8506aa
    keyId GUID for Verify: e7b8c96e-dec3-4023-9c8b-ff40fa7faa3a
    Password: 74a7e867-e4f1-49a5-82fe-2087bf53e7df
    displayName: CN=Example

    Public Key: MIIDAz...pJTZg==

    Cert thumprint: 14B73D02E5094675063DF66A42B914DAD71633D7

    customKeyIdentifier:
    dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=
    ```

- <span data-ttu-id="84a50-125">本教程的前提是使用 Microsoft Graph Explorer，但是可以使用 Postman，也可以创建自己的客户端应用程序来调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="84a50-125">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="84a50-126">如果要在本教程中调用 Microsoft Graph API，需要使用具有全局管理员角色和适当权限的帐户。</span><span class="sxs-lookup"><span data-stu-id="84a50-126">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="84a50-127">对于本教程，需要`Application.ReadWrite.All`、`AppRoleAssignment.ReadWrite.All`、`Policy.Read.All`和 `Policy.ReadWrite.ApplicationConfiguration` 委派权限。</span><span class="sxs-lookup"><span data-stu-id="84a50-127">For this tutorial, the `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All`, and `Policy.ReadWrite.ApplicationConfiguration` delegated permissions are needed.</span></span> <span data-ttu-id="84a50-128">完成以下步骤以在 Microsoft Graph Explorer 中设置权限：</span><span class="sxs-lookup"><span data-stu-id="84a50-128">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>

    1. <span data-ttu-id="84a50-129">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="84a50-129">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="84a50-130">选择“**使用 Microsoft 登录**”，然后使用 Azure AD 全局管理员账户登录。</span><span class="sxs-lookup"><span data-stu-id="84a50-130">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="84a50-131">成功登录后，可在左侧窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="84a50-131">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="84a50-132">选择用户帐户详细信息右侧的设置图标，然后选择“**权限**”。</span><span class="sxs-lookup"><span data-stu-id="84a50-132">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![选择 Microsoft Graph 权限](./images/application-saml-sso-configure-api/set-permissions.png)
        
    4. <span data-ttu-id="84a50-134">滚动权限列表至 `AppRoleAssignment` 权限，展开 **AppRoleAssignment (1)**，然后选择 **AppRoleAssignment.ReadWrite.All** 权限。</span><span class="sxs-lookup"><span data-stu-id="84a50-134">Scroll through the list of permissions to the `AppRoleAssignment` permissions, expand **AppRoleAssignment (1)**, and select the **AppRoleAssignment.ReadWrite.All** permission.</span></span> <span data-ttu-id="84a50-135">继续向下滚动权限列表至 `Application` 权限，展开 **应用 (2)**，然后选择 **Application.ReadWrite.All** 权限。</span><span class="sxs-lookup"><span data-stu-id="84a50-135">Scroll further down the list of permissions to the `Application` permissions, expand **Application (2)**, and select the **Application.ReadWrite.All** permission.</span></span> <span data-ttu-id="84a50-136">继续选择 `Policy` 权限，展开 **策略 (13)**，然后选择 **Policy.Read.All**  和 **Policy.ReadWrite.ApplicationConfiguration** 权限。</span><span class="sxs-lookup"><span data-stu-id="84a50-136">Continue to the `Policy` permissions, expand **Policy (13)**, and select the **Policy.Read.All**  and **Policy.ReadWrite.ApplicationConfiguration** permissions.</span></span>

        ![滚动并选择 approleasignment、应用程序和策略权限](./images/application-saml-sso-configure-api/select-permissions.png)

    5. <span data-ttu-id="84a50-138">选择“**同意**”，然后选择“**接受**”，以接受同意权限。</span><span class="sxs-lookup"><span data-stu-id="84a50-138">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="84a50-139">你不需要代表组织同意这些权限。</span><span class="sxs-lookup"><span data-stu-id="84a50-139">You do not need to consent on behalf of your organization for these permissions.</span></span>

        ![接受同意权限](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a><span data-ttu-id="84a50-141">第 1 步：创建应用程序</span><span class="sxs-lookup"><span data-stu-id="84a50-141">Step 1: Create the application</span></span>

<span data-ttu-id="84a50-142">Azure AD 中存在一个库，其中包含数千个预集成的应用程序，可以将其用作应用程序的模板。</span><span class="sxs-lookup"><span data-stu-id="84a50-142">Azure AD has a gallery that contains thousands of pre-integrated applications that you can use as a template for your application.</span></span> <span data-ttu-id="84a50-143">应用程序模板描述了该应用程序的元数据。</span><span class="sxs-lookup"><span data-stu-id="84a50-143">The application template describes the metadata for that application.</span></span> <span data-ttu-id="84a50-144">使用此模板，可以在租户中创建应用程序和服务主体的实例以进行管理。</span><span class="sxs-lookup"><span data-stu-id="84a50-144">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span> 

<span data-ttu-id="84a50-145">如果要从库中创建应用程序，首先获取应用程序模板的标识符，然后使用该标识符创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="84a50-145">To create the application from the gallery, you first get the identifier of the application template and then use that identifier to create the application.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="84a50-146">检索库应用程序模板标识符</span><span class="sxs-lookup"><span data-stu-id="84a50-146">Retrieve the gallery application template identifier</span></span>

 <span data-ttu-id="84a50-147">在本教程中，将检索 `Amazon Web Services (AWS)` 应用程序模板的标识符。</span><span class="sxs-lookup"><span data-stu-id="84a50-147">In this tutorial, you retrieve the identifier of the application template for `Amazon Web Services (AWS)`.</span></span> <span data-ttu-id="84a50-148">记录 **id** 属性值，以供稍后在本教程中使用。</span><span class="sxs-lookup"><span data-stu-id="84a50-148">Record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-149">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-149">Request</span></span>

```http
GET https://graph.microsoft.com/beta/applicationTemplates?$filter=displayName eq 'Amazon Web Services (AWS)'
```

#### <a name="response"></a><span data-ttu-id="84a50-150">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-150">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applicationTemplates",
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
        "developerServices",
        "topApps"
      ],
      "publisher": "Amazon",
      "description": null
    }
  ]
}
```

### <a name="create-the-application"></a><span data-ttu-id="84a50-151">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="84a50-151">Create the application</span></span>

<span data-ttu-id="84a50-152">使用为应用模板记录的 **id** 值，在租户中为应用和服务主题创建实例。</span><span class="sxs-lookup"><span data-stu-id="84a50-152">Using the **id** value that you recorded for the application template, create an instance of the application and service principal in your tenant.</span></span> <span data-ttu-id="84a50-153">记录应用程序的 **objectId** 属性值和服务主体的 **objectId** 属性值，以在本教程中稍后使用。</span><span class="sxs-lookup"><span data-stu-id="84a50-153">Record the value of the **objectId** property of the application and the value of the **objectId** property for the service principal to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-154">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-154">Request</span></span>

```http
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> <span data-ttu-id="84a50-155">留出一些时间将应用程序配置到 Azure AD 租户中。</span><span class="sxs-lookup"><span data-stu-id="84a50-155">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="84a50-156">这不是即时的。</span><span class="sxs-lookup"><span data-stu-id="84a50-156">It is not instant.</span></span> <span data-ttu-id="84a50-157">一种策略是每 5-10秒 对应用程序或服务主体对象执行 GET 查询，直到查询成功。</span><span class="sxs-lookup"><span data-stu-id="84a50-157">One strategy is to do a GET query on the application or service principal object every 5-10 seconds until the query is successful.</span></span>

#### <a name="response"></a><span data-ttu-id="84a50-158">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-158">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "objectId": "8f558912-0ca3-4f1e-ab6e-66ad7fa4e7bb",
    "appId": "536c33dc-dc28-42c8-ba1d-406524d83ec3",
    "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
    "displayName": "AWS Contoso",
    "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
    "identifierUris": [],
    "publicClient": null,
    "replyUrls": [
      "https://signin.aws.amazon.com/saml"
    ],
    "logoutUrl": null,
    "samlMetadataUrl": null,
    "errorUrl": null,
    "groupMembershipClaims": null,
    "availableToOtherTenants": false
  },
  "servicePrincipal": {
    "objectId": "3161ab85-8f57-4ae0-82d3-7a1f71680b27",
    "deletionTimestamp": null,
    "accountEnabled": true,
    "appId": "536c33dc-dc28-42c8-ba1d-406524d83ec3",
    "appDisplayName": "AWS Contoso",
    "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
    "appRoleAssignmentRequired": true,
    "displayName": "AWS Contoso",
    "errorUrl": null,
    "logoutUrl": null,
    "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
    "samlMetadataUrl": null,
    "microsoftFirstParty": null,
    "publisherName": "Contoso",
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [
      "https://signin.aws.amazon.com/saml"
    ],
    "servicePrincipalNames": [
      "536c33dc-dc28-42c8-ba1d-406524d83ec3"
    ],
    "tags": [
      "WindowsAzureActiveDirectoryIntegratedApp"
    ],
    "notificationEmailAddresses": [],
    "keyCredentials": [],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="84a50-159">第 2 步：配置单一登录</span><span class="sxs-lookup"><span data-stu-id="84a50-159">Step 2: Configure single sign-on</span></span>

<span data-ttu-id="84a50-160">在本教程中，`saml`设置为服务主体中的单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="84a50-160">In this tutorial, you set `saml` as the single sign-on mode in the service principal.</span></span> <span data-ttu-id="84a50-161">使用之前记录的服务主体 **objectId**。</span><span class="sxs-lookup"><span data-stu-id="84a50-161">Use the **objectId** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-162">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-162">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a><span data-ttu-id="84a50-163">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-163">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a><span data-ttu-id="84a50-164">设置基本 SAML URL</span><span class="sxs-lookup"><span data-stu-id="84a50-164">Set basic SAML URLs</span></span>

<span data-ttu-id="84a50-165">使用之前记录的应用 **objectId**，设置标识符 URI，并在应用对象中重新定向 AWS 的 URI。</span><span class="sxs-lookup"><span data-stu-id="84a50-165">Using the **objectId** for the application that you recorded earlier, set the identifier URI and redirect URI for AWS in the application object.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-166">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-166">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/applications/8f558912-0ca3-4f1e-ab6e-66ad7fa4e7bb
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

#### <a name="response"></a><span data-ttu-id="84a50-167">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-167">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a><span data-ttu-id="84a50-168">添加应用程序角色（可选）</span><span class="sxs-lookup"><span data-stu-id="84a50-168">Add app roles (Optional)</span></span>

<span data-ttu-id="84a50-169">如果应用程序需要令牌中的角色信息，请在应用程序对象中添加角色的定义。</span><span class="sxs-lookup"><span data-stu-id="84a50-169">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> 

> [!NOTE] 
> <span data-ttu-id="84a50-170">添加应用程序角色时，请勿修改默认应用程序角色 `msiam_access`。</span><span class="sxs-lookup"><span data-stu-id="84a50-170">When adding app roles, don't modify the default app roles `msiam_access`.</span></span> 

<span data-ttu-id="84a50-171">使用之前记录的服务主体 **objectId**。</span><span class="sxs-lookup"><span data-stu-id="84a50-171">Use the **objectId** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-172">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-172">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/serviceprincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
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

#### <a name="response"></a><span data-ttu-id="84a50-173">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-173">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="84a50-174">第 3 步：配置声明映射</span><span class="sxs-lookup"><span data-stu-id="84a50-174">Step 3: Configure claims mapping</span></span>

### <a name="create-a-claims-mapping-policy"></a><span data-ttu-id="84a50-175">创建声明映射策略</span><span class="sxs-lookup"><span data-stu-id="84a50-175">Create a claims mapping policy</span></span>

<span data-ttu-id="84a50-176">除了基本声明之外，还为 Azure AD 配置以下声明以在 SAML 令牌中发出：</span><span class="sxs-lookup"><span data-stu-id="84a50-176">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="84a50-177">声明名称</span><span class="sxs-lookup"><span data-stu-id="84a50-177">Claim name</span></span> | <span data-ttu-id="84a50-178">源</span><span class="sxs-lookup"><span data-stu-id="84a50-178">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="84a50-179">assignedroles</span><span class="sxs-lookup"><span data-stu-id="84a50-179">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="84a50-180">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="84a50-180">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="84a50-181">"900"</span><span class="sxs-lookup"><span data-stu-id="84a50-181">"900"</span></span> |
| <span data-ttu-id="84a50-182">roles</span><span class="sxs-lookup"><span data-stu-id="84a50-182">roles</span></span> | <span data-ttu-id="84a50-183">assignedroles</span><span class="sxs-lookup"><span data-stu-id="84a50-183">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="84a50-184">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="84a50-184">userprincipalname</span></span> |

> [!NOTE]
> <span data-ttu-id="84a50-185">声明映射策略中的某些项区分大小写（例如“Version”）。</span><span class="sxs-lookup"><span data-stu-id="84a50-185">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="84a50-186">如果收到错误消息，例如“属性的值无效”，则可能是区分大小写的问题。</span><span class="sxs-lookup"><span data-stu-id="84a50-186">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

<span data-ttu-id="84a50-187">创建声明映射策略并创建 **id**，以随后在本教程中使用。</span><span class="sxs-lookup"><span data-stu-id="84a50-187">Create the claims mapping policy and record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-188">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-188">Request</span></span>

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

#### <a name="response"></a><span data-ttu-id="84a50-189">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-189">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: claimsMappingPolicies/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/claimsMappingPolicies/$entity",
  "id": "218e7879-5330-4ca6-8bca-ddb1f2402e73",
  "deletedDateTime": null,
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a><span data-ttu-id="84a50-190">向服务主体分配声明映射策略</span><span class="sxs-lookup"><span data-stu-id="84a50-190">Assign a claims mapping policy to a service principal</span></span>

<span data-ttu-id="84a50-191">使用之前记录的服务主体 **objectId** 为其分配映射策略。</span><span class="sxs-lookup"><span data-stu-id="84a50-191">Use the **objectId** for the service principal that you recorded earlier to assign a claims mapping policy to it.</span></span> <span data-ttu-id="84a50-192">将 **id** 属性值用于请求正文中的声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="84a50-192">Use the value of the **id** property for the claims mapping policy in the body of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-193">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-193">Request</span></span>

```http
POST https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73"
}
```

#### <a name="response"></a><span data-ttu-id="84a50-194">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-194">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a><span data-ttu-id="84a50-195">第 4 步：配置签名证书</span><span class="sxs-lookup"><span data-stu-id="84a50-195">Step 4: Configure a signing certificate</span></span>

<span data-ttu-id="84a50-196">向应用程序分配证书。</span><span class="sxs-lookup"><span data-stu-id="84a50-196">Assign your certificate to the application.</span></span> 

#### <a name="request"></a><span data-ttu-id="84a50-197">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-197">Request</span></span>

<span data-ttu-id="84a50-198">在请求正文中，提供这些值：</span><span class="sxs-lookup"><span data-stu-id="84a50-198">In the request body, provide these values:</span></span>

<span data-ttu-id="84a50-199">**keyCredentials - 签名**</span><span class="sxs-lookup"><span data-stu-id="84a50-199">**keyCredentials - Sign**</span></span>

- <span data-ttu-id="84a50-200">**customKeyIdentifier** - 证书指纹的哈希。</span><span class="sxs-lookup"><span data-stu-id="84a50-200">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="84a50-201">**endDateTime** - 证书的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="84a50-201">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="84a50-202">**keyId** - 凭据的标识符。</span><span class="sxs-lookup"><span data-stu-id="84a50-202">**keyId** - The identifier for the credential.</span></span> <span data-ttu-id="84a50-203">与 **passwordCredentials** 的 keyId 相同。</span><span class="sxs-lookup"><span data-stu-id="84a50-203">Same as the keyId for the **passwordCredentials**.</span></span>
- <span data-ttu-id="84a50-204">**startDateTime** - 证书的开始日期。</span><span class="sxs-lookup"><span data-stu-id="84a50-204">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="84a50-205">**key** - 证书的 Base64 编码私钥。</span><span class="sxs-lookup"><span data-stu-id="84a50-205">**key** - The base-64 encoded private key of the certificate.</span></span>
- <span data-ttu-id="84a50-206">**displayName** - 凭据的显示名称。</span><span class="sxs-lookup"><span data-stu-id="84a50-206">**displayName** - The display name for the credentials.</span></span>

<span data-ttu-id="84a50-207">**keyCredentials - 验证**</span><span class="sxs-lookup"><span data-stu-id="84a50-207">**keyCredentials - Verify**</span></span>

- <span data-ttu-id="84a50-208">**customKeyIdentifier** - 证书指纹的哈希。</span><span class="sxs-lookup"><span data-stu-id="84a50-208">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="84a50-209">**endDateTime** - 证书的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="84a50-209">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="84a50-210">**keyId** - 凭据的标识符。</span><span class="sxs-lookup"><span data-stu-id="84a50-210">**keyId** - The identifier for the credential.</span></span>
- <span data-ttu-id="84a50-211">**startDateTime** - 证书的开始日期。</span><span class="sxs-lookup"><span data-stu-id="84a50-211">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="84a50-212">**key** - 证书的 Base64 编码公钥。</span><span class="sxs-lookup"><span data-stu-id="84a50-212">**key** - The base-64 encoded public key of the certificate.</span></span>
- <span data-ttu-id="84a50-213">**displayName** - 凭据的显示名称。</span><span class="sxs-lookup"><span data-stu-id="84a50-213">**displayName** - The display name for the credentials.</span></span>

<span data-ttu-id="84a50-214">**passwordCredentials**</span><span class="sxs-lookup"><span data-stu-id="84a50-214">**passwordCredentials**</span></span>

- <span data-ttu-id="84a50-215">**customKeyIdentifier** - 证书指纹的哈希。</span><span class="sxs-lookup"><span data-stu-id="84a50-215">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="84a50-216">**keyId** - 凭据的标识符。</span><span class="sxs-lookup"><span data-stu-id="84a50-216">**keyId** - The identifier for the credential.</span></span> <span data-ttu-id="84a50-217">与 **keyCredentials - 签名** 的 keyId 相同。</span><span class="sxs-lookup"><span data-stu-id="84a50-217">Same as the keyId for the **keyCredentials - Sign**.</span></span>
- <span data-ttu-id="84a50-218">**endDateTime** - 证书的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="84a50-218">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="84a50-219">**startDateTime** - 证书的开始日期。</span><span class="sxs-lookup"><span data-stu-id="84a50-219">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="84a50-220">**secretText** - 证书的密码。</span><span class="sxs-lookup"><span data-stu-id="84a50-220">**secretText** - The password for the certificate.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipals/json

{
  "keyCredentials":[
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "endDateTime": 2022-12-17T20:33:07.0000000Z",
      "keyId": "ed4f28e8-a502-4440-bfba-6038cb8506aa",
      "startDateTime": "2020-12-17T20:33:07.0000000Z",
      "type": "X509CertAndPassword",
      "usage": "Sign",
      "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
      "displayName": "CN=Example"
    },
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "endDateTime": "2022-12-17T20:33:07.0000000Z",
      "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
      "startDateTime": "2020-12-17T20:33:07.0000000Z",
      "type": "AsymmetricX509Cert",
      "usage": "Verify",
      "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
      "displayName": "CN=Example"
    }
  ],
  "passwordCredentials": [
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "keyId": "ed4f28e8-a502-4440-bfba-6038cb8506aa",
      "endDateTime": "2022-01-27T19:40:33Z",
      "startDateTime": "2020-04-20T19:40:33Z",
      "secretText": "74a7e867-e4f1-49a5-82fe-2087bf53e7df"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="84a50-221">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-221">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="84a50-222">激活自定义签名密钥</span><span class="sxs-lookup"><span data-stu-id="84a50-222">Activate the custom signing key</span></span>

<span data-ttu-id="84a50-223">需要将服务主体的 **preferredTokenSigningKeyThumbprint** 属性设置为想要Azure AD 用于签署 SAML 响应的证书指纹。</span><span class="sxs-lookup"><span data-stu-id="84a50-223">You need to set the **preferredTokenSigningKeyThumbprint** property of the service principal to the thumbprint of the certificate that you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="84a50-224">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-224">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "14B73D02E5094675063DF66A42B914DAD71633D7"
}
```

#### <a name="response"></a><span data-ttu-id="84a50-225">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-225">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a><span data-ttu-id="84a50-226">第 5 步：分配用户</span><span class="sxs-lookup"><span data-stu-id="84a50-226">Step 5: Assign users</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="84a50-227">创建用户账户</span><span class="sxs-lookup"><span data-stu-id="84a50-227">Create a user account</span></span>

<span data-ttu-id="84a50-228">对于本教程，将创建一个添加到应用程序中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="84a50-228">For this tutorial, you create a user account that is added to the application.</span></span> <span data-ttu-id="84a50-229">在请求正文中，将 contoso.com 更改为租户的域名。</span><span class="sxs-lookup"><span data-stu-id="84a50-229">In the request body, change contoso.com to the domain name of your tenant.</span></span> <span data-ttu-id="84a50-230">可在 Azure Active Directory 概述页面上找到租户信息。</span><span class="sxs-lookup"><span data-stu-id="84a50-230">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="84a50-231">记录要在本教程后面要使用的用户 **id**。</span><span class="sxs-lookup"><span data-stu-id="84a50-231">Record the **id** of the user to be used later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-232">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-232">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="84a50-233">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-233">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "mytestuser1@contoso.com"
}
```

### <a name="assign-a-user-to-the-application"></a><span data-ttu-id="84a50-234">向应用程序分配用户</span><span class="sxs-lookup"><span data-stu-id="84a50-234">Assign a user to the application</span></span>

<span data-ttu-id="84a50-235">将创建的用户分配给服务主体，然后分配 `Admin,WAAD` 应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="84a50-235">Assign the user that you created to the service principal and assign the `Admin,WAAD` app role.</span></span> 

<span data-ttu-id="84a50-236">在请求正文中，提供这些值：</span><span class="sxs-lookup"><span data-stu-id="84a50-236">In the request body, provide these values:</span></span>

- <span data-ttu-id="84a50-237">**principalId** - 所创建的用户账户的 **id**。</span><span class="sxs-lookup"><span data-stu-id="84a50-237">**principalId** - The **id** of the user account that you created.</span></span>
- <span data-ttu-id="84a50-238">**appRoleId** - 新增 `Admin,WAAD` 应用程序角色的 **id**。</span><span class="sxs-lookup"><span data-stu-id="84a50-238">**appRoleId** - The **id** of the `Admin,WAAD` app role that you added.</span></span>
- <span data-ttu-id="84a50-239">**resourceId** - 服务主体的 **id**。</span><span class="sxs-lookup"><span data-stu-id="84a50-239">**resourceId** - The **id** of the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-240">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-240">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"3161ab85-8f57-4ae0-82d3-7a1f71680b27"
}
```

#### <a name="response"></a><span data-ttu-id="84a50-241">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-241">Response</span></span>

```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('39406665-d521-40b7-9218-55070cae56b5')/appRoleAssignments/$entity",
  "id": "jKL4BeO2yUag4xULULSkza2HXRq_atpHrViBM89X55s",
  "deletedDateTime": null,
  "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
  "createdDateTime": "2021-02-11T22:51:36.8978032Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "05f8a28c-b6e3-46c9-a0e3-150b50b4a4cd",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "39406665-d521-40b7-9218-55070cae56b5"
}
```

## <a name="step-6-get-azure-ad-saml-metadata"></a><span data-ttu-id="84a50-242">第 6 步：获取 Azure AD SAML 元数据</span><span class="sxs-lookup"><span data-stu-id="84a50-242">Step 6: Get Azure AD SAML metadata</span></span>

<span data-ttu-id="84a50-243">使用以下 URL 获取特定配置的应用程序的 Azure AD SAML 元数据。</span><span class="sxs-lookup"><span data-stu-id="84a50-243">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="84a50-244">元数据包含诸如签名证书、Azure AD entityID和 Azure AD SingleSignOnService 等信息。</span><span class="sxs-lookup"><span data-stu-id="84a50-244">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

<span data-ttu-id="84a50-245">下面显示了可能在应用程序中看到的示例：</span><span class="sxs-lookup"><span data-stu-id="84a50-245">The following shows an example of what you might see for your application:</span></span>

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

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="84a50-246">第 7 步：清理资源</span><span class="sxs-lookup"><span data-stu-id="84a50-246">Step 7: Clean up resources</span></span>

<span data-ttu-id="84a50-247">在此步骤中，将删除创建的资源。</span><span class="sxs-lookup"><span data-stu-id="84a50-247">In this step, you remove the resources that you created.</span></span>


### <a name="delete-the-application"></a><span data-ttu-id="84a50-248">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="84a50-248">Delete the application</span></span>

<span data-ttu-id="84a50-249">删除创建的应用程序。</span><span class="sxs-lookup"><span data-stu-id="84a50-249">Delete the application that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-250">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-250">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/applications/4b01f51f-079b-4634-b767-7e19ad502cdb
```

#### <a name="response"></a><span data-ttu-id="84a50-251">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-251">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="84a50-252">删除用户账户</span><span class="sxs-lookup"><span data-stu-id="84a50-252">Delete the user account</span></span>

<span data-ttu-id="84a50-253">删除 MyTestUser1 用户帐户。</span><span class="sxs-lookup"><span data-stu-id="84a50-253">Delete the MyTestUser1 user account.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-254">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-254">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4
```

#### <a name="response"></a><span data-ttu-id="84a50-255">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-255">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a><span data-ttu-id="84a50-256">删除声明映射策略</span><span class="sxs-lookup"><span data-stu-id="84a50-256">Delete the claims mapping policy</span></span>

<span data-ttu-id="84a50-257">删除声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="84a50-257">Delete the claims mapping policy.</span></span>

#### <a name="request"></a><span data-ttu-id="84a50-258">请求</span><span class="sxs-lookup"><span data-stu-id="84a50-258">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73
```

#### <a name="response"></a><span data-ttu-id="84a50-259">响应</span><span class="sxs-lookup"><span data-stu-id="84a50-259">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="84a50-260">另请参阅</span><span class="sxs-lookup"><span data-stu-id="84a50-260">See also</span></span>

- <span data-ttu-id="84a50-261">对于 AWS，可以[启用用户配置](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)以从该 AWS 账户获取所有角色。</span><span class="sxs-lookup"><span data-stu-id="84a50-261">For AWS, you can [enable user provisioning](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> <span data-ttu-id="84a50-262">有关详细信息，请参阅[配置 SAML 令牌中颁发的角色声明](/azure/active-directory/develop/active-directory-enterprise-app-role-management)。</span><span class="sxs-lookup"><span data-stu-id="84a50-262">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>
- <span data-ttu-id="84a50-263">[自定义在租户具体应用的令牌中颁发的声明](/azure/active-directory/develop/active-directory-claims-mapping)。</span><span class="sxs-lookup"><span data-stu-id="84a50-263">[Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
- <span data-ttu-id="84a50-264">可以使用 applicationTemplate API 来实例化[非库应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal)。</span><span class="sxs-lookup"><span data-stu-id="84a50-264">You can use the applicationTemplate API to instantiate [Non-Gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="84a50-265">使用 applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`。</span><span class="sxs-lookup"><span data-stu-id="84a50-265">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>
- [<span data-ttu-id="84a50-266">New-SelfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="84a50-266">New-SelfSignedCertificate</span></span>](/powershell/module/pkiclient/new-selfsignedcertificate?view=win10-ps)
- [<span data-ttu-id="84a50-267">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="84a50-267">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-beta)
- [<span data-ttu-id="84a50-268">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="84a50-268">appRoleAssignment</span></span>](/graph/api/resources/approleassignment?view=graph-rest-1.0)
- [<span data-ttu-id="84a50-269">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="84a50-269">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [<span data-ttu-id="84a50-270">application</span><span class="sxs-lookup"><span data-stu-id="84a50-270">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
- [<span data-ttu-id="84a50-271">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="84a50-271">claimsMappingPolicy</span></span>](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)
- [<span data-ttu-id="84a50-272">keyCredential</span><span class="sxs-lookup"><span data-stu-id="84a50-272">keyCredential</span></span>](/graph/api/resources/keycredential?view=graph-rest-1.0)
