---
title: 将应用程序权限限制为特定 Exchange Online 邮箱
description: 若要将应用程序权限界定为特定 Exchange Online 邮箱，你需要创建应用程序访问策略。
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: e9f6b63f64981a49c655208c45ef9754324d5ae4
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456427"
---
# <a name="limiting-application-permissions-to-specific-exchange-online-mailboxes"></a><span data-ttu-id="fe450-103">将应用程序权限限制为特定 Exchange Online 邮箱</span><span class="sxs-lookup"><span data-stu-id="fe450-103">Limiting application permissions to specific Exchange Online mailboxes</span></span> 

<span data-ttu-id="fe450-104">想要限制对特定邮箱的应用访问权限的管理员可以使用 **New-ApplicationAccessPolicy** PowerShell cmdlet 创建应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="fe450-104">Administrators who want to limit app access to specific mailboxes can create an application access policy by using the **New-ApplicationAccessPolicy** PowerShell cmdlet.</span></span> <span data-ttu-id="fe450-105">本文介绍配置访问控制的基本步骤。</span><span class="sxs-lookup"><span data-stu-id="fe450-105">This article covers the basic steps to configure access control.</span></span> <span data-ttu-id="fe450-106">这些步骤仅适用于 Exchange Online 资源，不适用于其他 Microsoft Graph 工作负载。</span><span class="sxs-lookup"><span data-stu-id="fe450-106">These steps are specific to Exchange Online resources and do not apply to other Microsoft Graph workloads.</span></span> 

## <a name="background"></a><span data-ttu-id="fe450-107">背景</span><span class="sxs-lookup"><span data-stu-id="fe450-107">Background</span></span>
<span data-ttu-id="fe450-108">一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="fe450-108">Some apps call Microsoft Graph using their own identity and not on behalf of a user.</span></span> <span data-ttu-id="fe450-109">这些是在服务器上运行的后台服务或守护程序，不存在登录用户。</span><span class="sxs-lookup"><span data-stu-id="fe450-109">These are usually background services or daemon apps that run on a server without the presence of a signed-in user.</span></span> <span data-ttu-id="fe450-110">这些应用使用 [OAuth 2.0 客户端凭据授予流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)进行身份验证，并使用应用程序权限进行配置，默认情况下，这些应用可以访问 exchange Online 上组织中的 _所有_ 邮箱。</span><span class="sxs-lookup"><span data-stu-id="fe450-110">These apps make use of [OAuth 2.0 client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to authenticate and are configured with application permissions, which by default enable such apps to access _all_ mailboxes in a organization on Exchange Online.</span></span> <span data-ttu-id="fe450-111">例如， `Mail.Read` 应用程序权限允许应用在没有登录用户的情况下读取所有邮箱中的邮件。</span><span class="sxs-lookup"><span data-stu-id="fe450-111">For example, the `Mail.Read` application permission allows apps to read mail in all mailboxes without a signed-in user.</span></span> 

<span data-ttu-id="fe450-112">在某些情况下，管理员可能希望将应用限制为仅特定邮箱， _并非所有_ 组织中的 Exchange Online 邮箱。</span><span class="sxs-lookup"><span data-stu-id="fe450-112">There are scenarios where administrators may want to limit an app to only specific mailboxes and _not all_ Exchange Online mailboxes in the organization.</span></span> <span data-ttu-id="fe450-113">管理员可以通过将邮箱放入启用邮件的安全组来标识允许访问的邮箱集。</span><span class="sxs-lookup"><span data-stu-id="fe450-113">Administrators can identify the set of mailboxes to permit access by putting them in a mail-enabled security group.</span></span> <span data-ttu-id="fe450-114">然后，管理员可以通过创建用于访问该组的应用程序访问策略，将第三方应用访问权限限制为仅对该组的邮箱。</span><span class="sxs-lookup"><span data-stu-id="fe450-114">Administrators can then limit third-party app access to only that set of  mailboxes by creating an application access policy for access to that group.</span></span>

> [!NOTE]
> <span data-ttu-id="fe450-115">为组织配置应用程序访问策略后，该策略将应用于使用 Microsoft Graph API 或 Exchange Web 服务访问 Exchange Online 邮箱的任何应用。</span><span class="sxs-lookup"><span data-stu-id="fe450-115">Once an application access policy is configured for an organization, the policy applies to any app that uses the Microsoft Graph API or Exchange Web Services to access Exchange Online mailboxes.</span></span>

<span data-ttu-id="fe450-116">如以下 [支持的权限和其他资源](#supported-permissions-and-additional-resources) 部分中所述，应用程序访问策略限制已授予策略支持的任何Microsoft Graph或 Exchange Web 服务权限范围的应用的邮箱访问权限。</span><span class="sxs-lookup"><span data-stu-id="fe450-116">As further described in the [Supported permissions and additional resources](#supported-permissions-and-additional-resources) section below, application access policy restricts mailbox access for apps that have been granted any of the Microsoft Graph or Exchange Web Services permission scopes that the policy supports.</span></span>

## <a name="configure-applicationaccesspolicy"></a><span data-ttu-id="fe450-117">配置应用程序访问策略</span><span class="sxs-lookup"><span data-stu-id="fe450-117">Configure ApplicationAccessPolicy</span></span>

<span data-ttu-id="fe450-118">若要配置应用程序访问策略并限制应用程序权限的范围：</span><span class="sxs-lookup"><span data-stu-id="fe450-118">To configure an application access policy and limit the scope of application permissions:</span></span>
1.  <span data-ttu-id="fe450-p104">连接到 Exchange Online PowerShell。有关详细信息，请参见[连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="fe450-p104">Connect to Exchange Online PowerShell. For details, see [Connect to Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>

2.  <span data-ttu-id="fe450-121">标识应用客户端 ID 和限制应用可访问的启用邮件的安全组。</span><span class="sxs-lookup"><span data-stu-id="fe450-121">Identify the app’s client ID and a mail-enabled security group to restrict the app’s access to.</span></span>

    - <span data-ttu-id="fe450-122">在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。</span><span class="sxs-lookup"><span data-stu-id="fe450-122">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="fe450-123">创建新的启用邮件的安全组，或使用现有安全组并标识改组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="fe450-123">Create a new mail-enabled security group or use an existing one and identify the email address for the group.</span></span> 

3.  <span data-ttu-id="fe450-124">创建应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="fe450-124">Create an application access policy.</span></span> 

    <span data-ttu-id="fe450-125">运行以下命令，替换 **AppId**、 **PolicyScopeGroupId** 和 **Description** 的参数。</span><span class="sxs-lookup"><span data-stu-id="fe450-125">Run the following command, replacing the arguments for **AppId**, **PolicyScopeGroupId**, and **Description**.</span></span>
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  <span data-ttu-id="fe450-126">测试新建的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="fe450-126">Test the newly created application access policy.</span></span>

    <span data-ttu-id="fe450-127">运行以下命令，替换 **Identity** 的参数，并 **AppId**。</span><span class="sxs-lookup"><span data-stu-id="fe450-127">Run the following command, replacing the arguments for **Identity** and **AppId**.</span></span>
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    <span data-ttu-id="fe450-128">此命令的输出将会指示该应用是否有权访问 User1 的邮箱。</span><span class="sxs-lookup"><span data-stu-id="fe450-128">The output of this command will indicate whether the app has access to User1’s mailbox.</span></span>

><span data-ttu-id="fe450-129">**注意：在 Microsoft Graph REST API 调用中，应用程序访问策略变更需要 30 分钟才能生效。**</span><span class="sxs-lookup"><span data-stu-id="fe450-129">**Note: Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.**</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="fe450-130">受支持的权限和其他资源</span><span class="sxs-lookup"><span data-stu-id="fe450-130">Supported permissions and additional resources</span></span>

<span data-ttu-id="fe450-131">管理员可以使用 ApplicationAccessPolicy cmdlet 来控制已授予以下任一Microsoft Graph应用程序权限或 Exchange Web 服务权限的应用的邮箱访问权限。</span><span class="sxs-lookup"><span data-stu-id="fe450-131">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access of an app that has been granted any of the following Microsoft Graph application permissions or Exchange Web Services permissions.</span></span> 

<span data-ttu-id="fe450-132">Microsoft Graph应用程序权限：</span><span class="sxs-lookup"><span data-stu-id="fe450-132">Microsoft Graph application permissions:</span></span> 
- `Mail.Read`
- `Mail.ReadBasic`
- `Mail.ReadBasic.All`
- `Mail.ReadWrite`
- `Mail.Send`
- `MailboxSettings.Read`
- `MailboxSettings.ReadWrite`
- `Calendars.Read`
- `Calendars.ReadWrite`
- `Contacts.Read`
- `Contacts.ReadWrite`

<span data-ttu-id="fe450-133">Exchange Web 服务权限范围： `full_access_as_app`。</span><span class="sxs-lookup"><span data-stu-id="fe450-133">Exchange Web Services permission scope: `full_access_as_app`.</span></span>

<span data-ttu-id="fe450-134">有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="fe450-134">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true).</span></span> 


## <a name="handling-api-errors"></a><span data-ttu-id="fe450-135">处理 API 错误</span><span class="sxs-lookup"><span data-stu-id="fe450-135">Handling API errors</span></span>
<span data-ttu-id="fe450-136">当 API 调用访问因所配置的应用程序访问策略而遭拒时，你可能会遇到以下错误。</span><span class="sxs-lookup"><span data-stu-id="fe450-136">You might encounter the following error when an API call is denied access due to a configured application access policy.</span></span> 
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
<span data-ttu-id="fe450-137">如果应用Microsoft Graph API 调用返回此错误，请与组织的 Exchange Online 管理员协作，确保应用有权访问邮箱资源。</span><span class="sxs-lookup"><span data-stu-id="fe450-137">If the Microsoft Graph API calls from your app return this error, work with the Exchange Online administrator for the organization to ensure that your app has permission to access the mailbox resource.</span></span>



## <a name="see-also"></a><span data-ttu-id="fe450-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fe450-138">See also</span></span>

- [<span data-ttu-id="fe450-139">权限参考</span><span class="sxs-lookup"><span data-stu-id="fe450-139">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="fe450-140">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="fe450-140">New-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [<span data-ttu-id="fe450-141">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="fe450-141">Get-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [<span data-ttu-id="fe450-142">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="fe450-142">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [<span data-ttu-id="fe450-143">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="fe450-143">Set-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [<span data-ttu-id="fe450-144">Test-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="fe450-144">Test-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/test-applicationaccesspolicy)
- [<span data-ttu-id="fe450-145">EWS 中的应用程序访问策略支持</span><span class="sxs-lookup"><span data-stu-id="fe450-145">Application Access Policy Support in EWS</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/application-access-policy-support-in-ews/ba-p/2110361)
