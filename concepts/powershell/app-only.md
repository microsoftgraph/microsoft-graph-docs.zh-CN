---
title: 对 Microsoft Graph PowerShell SDK 使用仅限应用的身份验证
description: 了解如何使用仅应用程序身份验证在 Microsoft Graph PowerShell SDK 中启用非交互应用场景。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 5e43072844193a7d971027e7e5368e4782c32e54
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193697"
---
# <a name="use-app-only-authentication-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="837ad-103">对 Microsoft Graph PowerShell SDK 使用仅限应用的身份验证</span><span class="sxs-lookup"><span data-stu-id="837ad-103">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="837ad-104">PowerShell SDK 支持两种类型的身份验证： [委派访问](..\auth-v2-user.md)权限和 [仅限应用访问](..\auth-v2-service.md)。</span><span class="sxs-lookup"><span data-stu-id="837ad-104">The PowerShell SDK supports two types of authentication: [delegated access](..\auth-v2-user.md), and [app-only access](..\auth-v2-service.md).</span></span> <span data-ttu-id="837ad-105">本指南将重点介绍启用仅限应用访问权限所需的配置。</span><span class="sxs-lookup"><span data-stu-id="837ad-105">This guide will focus on the configuration needed to enable app-only access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="837ad-106">仅限应用访问权限向应用程序直接授予权限，并要求管理员同意所需的权限范围。</span><span class="sxs-lookup"><span data-stu-id="837ad-106">App-only access grants permissions directly to an application, and requires an administrator to consent to the required permission scopes.</span></span> <span data-ttu-id="837ad-107">有关仅限应用访问权限的详细信息，请参阅 [Microsoft identity platform 和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="837ad-107">For more details on app-only access, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

<span data-ttu-id="837ad-108">我们来演练如何为简单脚本配置仅应用程序访问权限，以列出 Microsoft 365 租户中的用户和组。</span><span class="sxs-lookup"><span data-stu-id="837ad-108">Let's walk through configuring app-only access for a simple script to list users and groups in your Microsoft 365 tenant.</span></span>

## <a name="configuration"></a><span data-ttu-id="837ad-109">配置</span><span class="sxs-lookup"><span data-stu-id="837ad-109">Configuration</span></span>

<span data-ttu-id="837ad-110">在使用仅限应用访问的 SDK 之前，您需要具备以下各项。</span><span class="sxs-lookup"><span data-stu-id="837ad-110">Before you can use app-only access with the SDK, you need the following.</span></span>

- <span data-ttu-id="837ad-111">证书用作应用程序的凭据。</span><span class="sxs-lookup"><span data-stu-id="837ad-111">A certificate to use as a credential for the application.</span></span> <span data-ttu-id="837ad-112">这可以是自签名证书或来自颁发机构的证书。</span><span class="sxs-lookup"><span data-stu-id="837ad-112">This can be a self-signed certificate or a certificate from an authority.</span></span>
- <span data-ttu-id="837ad-113">您必须在 Azure AD 中 [注册应用程序](/azure/active-directory/develop/app-objects-and-service-principals) ，并使用您的方案所需的权限范围进行配置，并共享证书的公钥。</span><span class="sxs-lookup"><span data-stu-id="837ad-113">You must [register an application](/azure/active-directory/develop/app-objects-and-service-principals) in Azure AD, configure it with the permission scopes your scenario requires, and share the public key for your certificate.</span></span>

### <a name="certificate"></a><span data-ttu-id="837ad-114">证书</span><span class="sxs-lookup"><span data-stu-id="837ad-114">Certificate</span></span>

<span data-ttu-id="837ad-115">您将需要在将运行脚本的计算机上安装在用户的受信任存储区中的 x.509 证书。</span><span class="sxs-lookup"><span data-stu-id="837ad-115">You will need an X.509 certificate installed in your user's trusted store on the machine where you will run the script.</span></span> <span data-ttu-id="837ad-116">您还需要以 .cer、pem 或 .crt 格式导出的证书公钥。</span><span class="sxs-lookup"><span data-stu-id="837ad-116">You'll also need the certificate's public key exported in .cer, .pem, or .crt format.</span></span> <span data-ttu-id="837ad-117">你将需要证书主题的值。</span><span class="sxs-lookup"><span data-stu-id="837ad-117">You'll need the value of the certificate subject.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="837ad-118">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="837ad-118">Register the application</span></span>

<span data-ttu-id="837ad-119">你可以在 [Azure Active Directory 门户](https://aad.portal.azure.com)中或使用 PowerShell 注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="837ad-119">You can register the application either in the [Azure Active Directory portal](https://aad.portal.azure.com), or using PowerShell.</span></span>

# <a name="portal"></a>[<span data-ttu-id="837ad-120">门户</span><span class="sxs-lookup"><span data-stu-id="837ad-120">Portal</span></span>](#tab/azure-portal)

1. <span data-ttu-id="837ad-121">打开浏览器并导航到 [Azure Active Directory 管理中心](https://aad.portal.azure.com) ，并使用 Microsoft 365 租户组织管理员登录。</span><span class="sxs-lookup"><span data-stu-id="837ad-121">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using an Microsoft 365 tenant organization admin.</span></span>

1. <span data-ttu-id="837ad-122">选择左侧导航栏中的“**Azure Active Directory**”，再选择“**管理**”下的“**应用注册**”。</span><span class="sxs-lookup"><span data-stu-id="837ad-122">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

    ![<span data-ttu-id="837ad-123">应用注册的屏幕截图</span><span class="sxs-lookup"><span data-stu-id="837ad-123">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="837ad-124">选择“新注册”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="837ad-124">Select **New registration**.</span></span> <span data-ttu-id="837ad-125">在“注册应用”\*\*\*\* 页上，按如下方式设置值。</span><span class="sxs-lookup"><span data-stu-id="837ad-125">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="837ad-126">将“名称”\*\*\*\* 设置为“`Graph PowerShell Script`”。</span><span class="sxs-lookup"><span data-stu-id="837ad-126">Set **Name** to `Graph PowerShell Script`.</span></span>
    - <span data-ttu-id="837ad-127">仅将 **受支持的帐户类型** 设置为 **此组织目录中的帐户**。</span><span class="sxs-lookup"><span data-stu-id="837ad-127">Set **Supported account types** to **Accounts in this organizational directory only**.</span></span>
    - <span data-ttu-id="837ad-128">将 **重定向 URI** 保留为空。</span><span class="sxs-lookup"><span data-stu-id="837ad-128">Leave **Redirect URI** blank.</span></span>

    !["注册应用程序" 页的屏幕截图](./images/register-app.png)

1. <span data-ttu-id="837ad-130">选择“**注册**”。</span><span class="sxs-lookup"><span data-stu-id="837ad-130">Select **Register**.</span></span> <span data-ttu-id="837ad-131">在 " **图形 PowerShell 脚本** " 页面上，将应用程序的值复制 \*\* (客户端) id\*\* 和 **目录 (租户) id** 并保存它们。</span><span class="sxs-lookup"><span data-stu-id="837ad-131">On the **Graph PowerShell Script** page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them.</span></span>

    ![新应用注册的应用程序 ID 的屏幕截图](./images/aad-application-id.png)

1. <span data-ttu-id="837ad-133">选择 "**管理**" 下的 " **API 权限**"。</span><span class="sxs-lookup"><span data-stu-id="837ad-133">Select **API Permissions** under **Manage**.</span></span> <span data-ttu-id="837ad-134">选择 " **添加权限**"。</span><span class="sxs-lookup"><span data-stu-id="837ad-134">Choose **Add a permission**.</span></span>

1. <span data-ttu-id="837ad-135">依次选择 " **Microsoft Graph**" 和 " **应用程序权限**"。</span><span class="sxs-lookup"><span data-stu-id="837ad-135">Select **Microsoft Graph**, then **Application Permissions**.</span></span> <span data-ttu-id="837ad-136">添加 **用户。 read. all** 和 **Group. all**，然后选择 " **添加权限**"。</span><span class="sxs-lookup"><span data-stu-id="837ad-136">Add **User.Read.All** and **Group.Read.All**, then select **Add permissions**.</span></span>

1. <span data-ttu-id="837ad-137">在 **配置的权限**中，删除委派的 **用户。** 在 **Microsoft Graph** 下，选择权限右侧的 " **...** "，然后选择 " **删除权限**" 来读取权限。</span><span class="sxs-lookup"><span data-stu-id="837ad-137">In the **Configured permissions**, remove the delegated **User.Read** permission under **Microsoft Graph** by selecting the **...** to the right of the permission and selecting **Remove permission**.</span></span> <span data-ttu-id="837ad-138">选择 **"是，删除** 以确认"。</span><span class="sxs-lookup"><span data-stu-id="837ad-138">Select **Yes, remove** to confirm.</span></span>

1. <span data-ttu-id="837ad-139">选择 " **授予管理员同意 ...** " 按钮，然后选择 **"是"** 授予管理员同意配置的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="837ad-139">Select the **Grant admin consent for...** button, then select **Yes** to grant admin consent for the configured application permissions.</span></span> <span data-ttu-id="837ad-140">"**已配置权限**" 表中的 "**状态**" 列更改为 "已**授予"。**</span><span class="sxs-lookup"><span data-stu-id="837ad-140">The **Status** column in the **Configured permissions** table changes to **Granted for ...**.</span></span>

    ![授予了管理员同意的 webhook 的已配置权限的屏幕截图](./images/configured-permissions.png)

1. <span data-ttu-id="837ad-142">选择“管理”\*\*\*\* 下的“证书和密码”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="837ad-142">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="837ad-143">选择 " **上传证书** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="837ad-143">Select the **Upload certificate** button.</span></span> <span data-ttu-id="837ad-144">浏览到证书的公钥文件，然后选择 " **添加**"。</span><span class="sxs-lookup"><span data-stu-id="837ad-144">Browse to your certificate's public key file and select **Add**.</span></span>

# <a name="powershell"></a>[<span data-ttu-id="837ad-145">PowerShell</span><span class="sxs-lookup"><span data-stu-id="837ad-145">PowerShell</span></span>](#tab/powershell)

> [!NOTE]
> <span data-ttu-id="837ad-146">在执行以下步骤之前，您必须已 [安装](installation.md) Microsoft GRAPH PowerShell SDK。</span><span class="sxs-lookup"><span data-stu-id="837ad-146">You must have the Microsoft Graph PowerShell SDK [installed](installation.md) before following these steps.</span></span>

<span data-ttu-id="837ad-147">您可能想知道： "我可以使用 PowerShell SDK 注册应用程序，以便我可以使用 PowerShell SDK 吗？"</span><span class="sxs-lookup"><span data-stu-id="837ad-147">You may be wondering: "I can use the PowerShell SDK to register an app, so that I can use the PowerShell SDK?"</span></span> <span data-ttu-id="837ad-148">是的！</span><span class="sxs-lookup"><span data-stu-id="837ad-148">Yes!</span></span> <span data-ttu-id="837ad-149">在这种情况下，您使用的是具有委派访问权限的 PowerShell SDK，以管理员身份登录，并创建应用注册。</span><span class="sxs-lookup"><span data-stu-id="837ad-149">In this case, you're using the PowerShell SDK with delegated access, logging in as an administrator, and creating the app registration.</span></span> <span data-ttu-id="837ad-150">然后，使用该应用注册，可以将 PowerShell SDK 与仅限应用访问权限一起使用，以允许无人参与的脚本。</span><span class="sxs-lookup"><span data-stu-id="837ad-150">Then, using that app registration, you're able to use the PowerShell SDK with app-only access, allowing for unattended scripts.</span></span>

1. <span data-ttu-id="837ad-151">使用文本编辑器创建一个名为 **RegisterAppOnly.ps1**的新文件。</span><span class="sxs-lookup"><span data-stu-id="837ad-151">Use a text editor to create a new file named **RegisterAppOnly.ps1**.</span></span> <span data-ttu-id="837ad-152">将以下代码粘贴到文件中。</span><span class="sxs-lookup"><span data-stu-id="837ad-152">Paste the following code into the file.</span></span>

    :::code language="powershell" source="RegisterAppOnly.ps1":::

1. <span data-ttu-id="837ad-153">保存文件。</span><span class="sxs-lookup"><span data-stu-id="837ad-153">Save the file.</span></span> <span data-ttu-id="837ad-154">在包含 **RegisterAppOnly.ps1** 的目录中打开 PowerShell，并运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="837ad-154">Open PowerShell in the directory that contains **RegisterAppOnly.ps1** and run the following command.</span></span>

    ```powershell
    .\RegisterAppOnly.ps1 -AppName "Graph PowerShell Script" -CertPath "PATH_TO_PUBLIC_KEY_FILE"
    ```

1. <span data-ttu-id="837ad-155">根据提示打开浏览器。</span><span class="sxs-lookup"><span data-stu-id="837ad-155">Open your browser as prompted.</span></span> <span data-ttu-id="837ad-156">使用管理员帐户登录，并接受这些权限。</span><span class="sxs-lookup"><span data-stu-id="837ad-156">Sign in with an administrator account and accept the permissions.</span></span>

1. <span data-ttu-id="837ad-157">查看提示的输出 `Please go to the following URL in your browser to provide admin consent` 。</span><span class="sxs-lookup"><span data-stu-id="837ad-157">Review the output for the prompt `Please go to the following URL in your browser to provide admin consent`.</span></span> <span data-ttu-id="837ad-158">复制提供的 URL 并将其粘贴到浏览器中。</span><span class="sxs-lookup"><span data-stu-id="837ad-158">Copy the URL provided and paste it in your browser.</span></span> <span data-ttu-id="837ad-159">使用管理员帐户登录以授予对新注册应用程序的管理员同意。</span><span class="sxs-lookup"><span data-stu-id="837ad-159">Sign in with an administrator account to grant admin consent to your newly registered application.</span></span>

    > [!NOTE]
    > <span data-ttu-id="837ad-160">授予管理员同意后，浏览器将显示错误： `AADSTS500113: No reply address is registered for the application` 。</span><span class="sxs-lookup"><span data-stu-id="837ad-160">After granting admin consent, the browser will display an error: `AADSTS500113: No reply address is registered for the application`.</span></span> <span data-ttu-id="837ad-161">这是因为应用注册不包含重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="837ad-161">This is because the app registration does not include a redirect URL.</span></span> <span data-ttu-id="837ad-162">可以忽略此错误。</span><span class="sxs-lookup"><span data-stu-id="837ad-162">This error can be ignored.</span></span>

1. <span data-ttu-id="837ad-163">查看 PowerShell 输出的其余部分 `Connect-Graph` 预填充了您的应用程序注册值的命令。</span><span class="sxs-lookup"><span data-stu-id="837ad-163">Review the rest of the PowerShell output for `Connect-Graph` command pre-filled with the values for your app registration.</span></span>

---

## <a name="authenticate"></a><span data-ttu-id="837ad-164">身份验证</span><span class="sxs-lookup"><span data-stu-id="837ad-164">Authenticate</span></span>

<span data-ttu-id="837ad-165">完成上述配置步骤后，您应具有三条信息。</span><span class="sxs-lookup"><span data-stu-id="837ad-165">You should have three pieces of information after completing the configuration steps above.</span></span>

- <span data-ttu-id="837ad-166">上载到 Azure AD 应用注册的证书的证书主题。</span><span class="sxs-lookup"><span data-stu-id="837ad-166">Certificate subject of the certificate uploaded to your Azure AD app registration.</span></span>
- <span data-ttu-id="837ad-167">应用注册的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="837ad-167">Application ID for your app registration.</span></span>
- <span data-ttu-id="837ad-168">你的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="837ad-168">Your tenant ID.</span></span>

<span data-ttu-id="837ad-169">让我们使用它们来测试身份验证。</span><span class="sxs-lookup"><span data-stu-id="837ad-169">Let's use those to test authentication.</span></span> <span data-ttu-id="837ad-170">打开 PowerShell 并运行以下命令，将占位符替换为您的信息。</span><span class="sxs-lookup"><span data-stu-id="837ad-170">Open PowerShell and run the following command, replacing the placeholders with your information.</span></span>

```powershell
Connect-Graph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT
```

<span data-ttu-id="837ad-171">如果成功，你将看到 "" `Welcome To Microsoft Graph!` 。</span><span class="sxs-lookup"><span data-stu-id="837ad-171">If this succeeds, you will see `Welcome To Microsoft Graph!`.</span></span> <span data-ttu-id="837ad-172">运行 `Get-MgContext` 以验证您是否已通过仅限应用进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="837ad-172">Run `Get-MgContext` to verify that you've authenticated with app-only.</span></span> <span data-ttu-id="837ad-173">输出的外观应如下所示。</span><span class="sxs-lookup"><span data-stu-id="837ad-173">The output should look like the following.</span></span>

```powershell
ClientId              : YOUR_APP_ID
TenantId              : YOUR_TENANT_ID
CertificateThumbprint :
Scopes                : {Group.Read.All, User.Read.All}
AuthType              : AppOnly
CertificateName       : YOUR_CERT_SUBJECT
Account               :
AppName               : Graph PowerShell Script
ContextScope          : Process
```

## <a name="create-the-script"></a><span data-ttu-id="837ad-174">创建脚本</span><span class="sxs-lookup"><span data-stu-id="837ad-174">Create the script</span></span>

<span data-ttu-id="837ad-175">创建一个名为 **GraphAppOnly.ps1** 的新文件，并添加以下代码。</span><span class="sxs-lookup"><span data-stu-id="837ad-175">Create a new file named **GraphAppOnly.ps1** and add the following code.</span></span>

```powershell
# Authenticate
Connect-Graph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT

Write-Host "USERS:"
Write-Host "======================================================"
# List first 50 users
Get-MgUser -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

Write-Host "GROUPS:"
Write-Host "======================================================"
# List first 50 groups
Get-MgGroup -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

# Disconnect
Disconnect-Graph
```

<span data-ttu-id="837ad-176">将命令中的占位符替换 `Connect-Graph` 为您的信息。</span><span class="sxs-lookup"><span data-stu-id="837ad-176">Replace the placeholders in the `Connect-Graph` command with your information.</span></span> <span data-ttu-id="837ad-177">保存该文件，然后在创建该文件的目录中打开 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="837ad-177">Save the file, then open PowerShell in the directory where you created the file.</span></span> <span data-ttu-id="837ad-178">使用以下命令运行脚本。</span><span class="sxs-lookup"><span data-stu-id="837ad-178">Run the script with the following command.</span></span>

```powershell
.\GraphAppOnly.ps1
```

<span data-ttu-id="837ad-179">该脚本输出用户和组的列表，该列表类似于 (截断以简化) 的以下输出。</span><span class="sxs-lookup"><span data-stu-id="837ad-179">The script outputs a list of users and groups similar to the output below (truncated for brevity).</span></span>

```powershell
Welcome To Microsoft Graph!
USERS:
======================================================

DisplayName              Id
-----------              --
Conf Room Adams          88d1ba68-8ff5-4de2-90ed-768c00abcfae
Adele Vance              3103c7b9-cfe6-4cd3-a696-f88909b9a609
MOD Administrator        da3a885e-2d97-41de-9347-5271ef321b58
...

GROUPS:
======================================================

DisplayName                         Id
-----------                         --
App Development                     06dce3e5-d310-4add-ab2c-be728fb9076e
All Employees                       1a1cd42d-9801-4e9d-9b77-5215886174ef
Mark 8 Project Team                 2bf1b0d0-81f6-4e80-b971-d1db69f8d651
...
```
