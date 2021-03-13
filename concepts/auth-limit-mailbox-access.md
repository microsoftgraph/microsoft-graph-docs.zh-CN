---
title: 将应用程序权限界定为特定 Exchange Online 邮箱
description: 若要将应用程序权限界定为特定 Exchange Online 邮箱，你需要创建应用程序访问策略。
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: 56b05834f85c0b4a3f4480855cd0bffc8415b628
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760740"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a><span data-ttu-id="2d4d9-103">将应用程序权限界定为特定 Exchange Online 邮箱</span><span class="sxs-lookup"><span data-stu-id="2d4d9-103">Scoping application permissions to specific Exchange Online mailboxes</span></span> 

<span data-ttu-id="2d4d9-104">一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-104">Some apps call Microsoft Graph using their own identity and not on behalf of a user.</span></span> <span data-ttu-id="2d4d9-105">这些是在服务器上运行的后台服务或守护程序，不存在登录用户。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-105">These are usually background services or daemon apps that run on a server without the presence of a signed-in user.</span></span> <span data-ttu-id="2d4d9-106">这些应用使用 [OAuth 2.0 客户端凭据授权流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)来进行身份验证并配置应用程序权限，这使得这些应用能够访问组织在 Exchange Online 上的所有邮箱。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-106">These apps make use of [OAuth 2.0 client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to authenticate and are configured with application permissions, which enable such apps to access all mailboxes in a organization on Exchange Online.</span></span> <span data-ttu-id="2d4d9-107">例如，Mail.Read 应用程序权限使应用能够读取所有邮箱中的邮件而无需用户登录。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-107">For example, the Mail.Read application permission allows apps to read mail in all mailboxes without a signed-in user.</span></span> 

<span data-ttu-id="2d4d9-108">管理员如果想要将应用限制为访问特定邮箱集，则可以使用 **New-ApplicationAccessPolicy** PowerShell cmdlet 来配置访问权限。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-108">Administrators who want to limit the app access to a specific set of mailboxes can use the **New-ApplicationAccessPolicy** PowerShell cmdlet to configure access control.</span></span> <span data-ttu-id="2d4d9-109">本文介绍了配置应用程序访问策略的基本步骤。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-109">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="2d4d9-110">这些步骤仅适用于 Exchange Online 资源，不适用于其他 Microsoft Graph 工作负载。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-110">These steps are specific to Exchange Online resources and do not apply to other Microsoft Graph workloads.</span></span> 

## <a name="configure-applicationaccesspolicy"></a><span data-ttu-id="2d4d9-111">配置应用程序访问策略</span><span class="sxs-lookup"><span data-stu-id="2d4d9-111">Configure ApplicationAccessPolicy</span></span>

<span data-ttu-id="2d4d9-112">若要配置应用程序访问策略并限制应用程序权限的范围：</span><span class="sxs-lookup"><span data-stu-id="2d4d9-112">To configure an application access policy and limit the scope of application permissions:</span></span>
1.  <span data-ttu-id="2d4d9-113">连接到 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-113">Connect to Exchange Online PowerShell.</span></span> <span data-ttu-id="2d4d9-114">有关详细信息，请参阅[连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-114">For details, see [Connect to Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2.  <span data-ttu-id="2d4d9-115">标识应用客户端 ID 和限制应用可访问的启用邮件的安全组。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-115">Identify the app’s client ID and a mail-enabled security group to restrict the app’s access to.</span></span>

    - <span data-ttu-id="2d4d9-116">在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-116">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="2d4d9-117">创建新的启用邮件的安全组，或使用现有安全组并标识改组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-117">Create a new mail-enabled security group or use an existing one and identify the email address for the group.</span></span> 

3.  <span data-ttu-id="2d4d9-118">创建应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-118">Create an application access policy.</span></span> 

    <span data-ttu-id="2d4d9-119">运行以下命令，以替换 **AppId**、**PolicyScopeGroupId** 和 **Description** 参数。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-119">Run the following command, replacing the **AppId**, **PolicyScopeGroupId**, and **Description** arguments.</span></span>
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  <span data-ttu-id="2d4d9-120">测试新建的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-120">Test the newly created application access policy.</span></span>

    <span data-ttu-id="2d4d9-121">运行以下命令，以替换 **AppId** 和 **Identity** 参数。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-121">Run the following command, replacing the **AppId** and **Identity** arguments.</span></span>
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    <span data-ttu-id="2d4d9-122">此命令的输出将会指示该应用是否有权访问 User1 的邮箱。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-122">The output of this command will indicate whether the app has access to User1’s mailbox.</span></span>

<span data-ttu-id="2d4d9-123">注意：在 Microsoft Graph REST API 调用中，应用程序访问策略变更需要 30 分钟才能生效。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-123">Note: Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="2d4d9-124">受支持的权限和其他资源</span><span class="sxs-lookup"><span data-stu-id="2d4d9-124">Supported permissions and additional resources</span></span>
<span data-ttu-id="2d4d9-125">管理员可以使用 ApplicationAccessPolicy cmdlet 来控制已授权以下任何应用程序权限的应用的邮箱访问权限：</span><span class="sxs-lookup"><span data-stu-id="2d4d9-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access of an app that has been granted any of the following application permissions:</span></span> 
- <span data-ttu-id="2d4d9-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2d4d9-126">Mail.Read</span></span>
- <span data-ttu-id="2d4d9-127">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2d4d9-127">Mail.ReadBasic</span></span>
- <span data-ttu-id="2d4d9-128">Mail.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="2d4d9-128">Mail.ReadBasic.All</span></span>
- <span data-ttu-id="2d4d9-129">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d4d9-129">Mail.ReadWrite</span></span>
- <span data-ttu-id="2d4d9-130">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2d4d9-130">Mail.Send</span></span>
- <span data-ttu-id="2d4d9-131">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="2d4d9-131">MailboxSettings.Read</span></span>  
- <span data-ttu-id="2d4d9-132">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d4d9-132">MailboxSettings.ReadWrite</span></span>
- <span data-ttu-id="2d4d9-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2d4d9-133">Calendars.Read</span></span>
- <span data-ttu-id="2d4d9-134">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d4d9-134">Calendars.ReadWrite</span></span>
- <span data-ttu-id="2d4d9-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2d4d9-135">Contacts.Read</span></span>
- <span data-ttu-id="2d4d9-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d4d9-136">Contacts.ReadWrite</span></span>

<span data-ttu-id="2d4d9-137">有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/exchange/organization/new-applicationaccesspolicy)。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-137">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy).</span></span> 

## <a name="handling-api-errors"></a><span data-ttu-id="2d4d9-138">处理 API 错误</span><span class="sxs-lookup"><span data-stu-id="2d4d9-138">Handling API errors</span></span>
<span data-ttu-id="2d4d9-139">当 API 调用访问因所配置的应用程序访问策略而遭拒时，你可能会遇到以下错误。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-139">You might encounter the following error when an API call is denied access due to a configured application access policy.</span></span> 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
<span data-ttu-id="2d4d9-140">如果应用的 Microsoft Graph API 调用返回此错误，请与组织的 Exchange Online 管理员协作，确保你的应用具有邮箱资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="2d4d9-140">If Microsoft Graph API calls from your app return this error, work with the Exchange Online administrator for the organization to ensure that your app has permission to access the mailbox resource.</span></span>



## <a name="see-also"></a><span data-ttu-id="2d4d9-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2d4d9-141">See also</span></span>

- [<span data-ttu-id="2d4d9-142">权限参考</span><span class="sxs-lookup"><span data-stu-id="2d4d9-142">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="2d4d9-143">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2d4d9-143">New-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [<span data-ttu-id="2d4d9-144">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2d4d9-144">Get-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [<span data-ttu-id="2d4d9-145">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2d4d9-145">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [<span data-ttu-id="2d4d9-146">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2d4d9-146">Set-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [<span data-ttu-id="2d4d9-147">Test-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2d4d9-147">Test-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/test-applicationaccesspolicy)