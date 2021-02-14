---
title: 允许应用程序代表用户访问联机会议
description: 了解如何配置应用程序以代表用户访问联机会议。
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 46a91349a6a19b0caab62c6ea9712a3b5d798ac3
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239287"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="5f810-103">允许应用程序代表用户访问联机会议</span><span class="sxs-lookup"><span data-stu-id="5f810-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="5f810-104">在某些情况下，例如对于在服务器上运行的后台服务或守护程序应用（在没有登录用户的情况下运行）应用，应用可以调用 Microsoft Graph 代表用户执行操作。</span><span class="sxs-lookup"><span data-stu-id="5f810-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="5f810-105">例如，应用可能需要调用 Microsoft Graph，以根据已发布的计划安排多个会议 (如课程) 或外部计划工具。</span><span class="sxs-lookup"><span data-stu-id="5f810-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="5f810-106">在这些情况下，应用程序代表的用户被标识为会议组织者。</span><span class="sxs-lookup"><span data-stu-id="5f810-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="5f810-107">希望允许应用程序代表用户访问联机会议资源的管理员可以使用 **New-CsApplicationAccessPolicy** 和 **Grant-CsApplicationAccessPolicy** PowerShell cmdlet 配置访问控制。</span><span class="sxs-lookup"><span data-stu-id="5f810-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="5f810-108">本文介绍了配置应用程序访问策略的基本步骤。</span><span class="sxs-lookup"><span data-stu-id="5f810-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="5f810-109">这些步骤特定于联机会议，不适用于其他 Microsoft Graph 资源。</span><span class="sxs-lookup"><span data-stu-id="5f810-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="5f810-110">配置应用程序访问策略</span><span class="sxs-lookup"><span data-stu-id="5f810-110">Configure application access policy</span></span>

<span data-ttu-id="5f810-111">若要配置应用程序访问策略并允许应用程序使用应用程序权限访问联机会议，</span><span class="sxs-lookup"><span data-stu-id="5f810-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="5f810-112">标识应用的应用 (客户端) ID 以及将授权应用访问联机会议的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="5f810-112">Identify the app’s applcation (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="5f810-113">在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。</span><span class="sxs-lookup"><span data-stu-id="5f810-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="5f810-114">在 Azure 用户管理门户中 (用户) 对象 [ID](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="5f810-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="5f810-115">使用管理员帐户连接到 Skype for Business PowerShell。</span><span class="sxs-lookup"><span data-stu-id="5f810-115">Connect to Skype for Business PowerShell with an administrator account.</span></span> <span data-ttu-id="5f810-116">有关详细信息，请参阅使用 PowerShell 管理[Skype for Business Online。](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="5f810-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="5f810-117">创建包含应用 ID 列表的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="5f810-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="5f810-118">运行以下 cmdlet，将 **Identity、AppId\*\*\*\*和** **Description** (可选) 参数。</span><span class="sxs-lookup"><span data-stu-id="5f810-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="5f810-119">向用户授予策略，以允许策略中包含的应用 ID 代表授予的用户访问联机会议。</span><span class="sxs-lookup"><span data-stu-id="5f810-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="5f810-120">运行以下 cmdlet，替换 **PolicyName** 和 **Identity** 参数。</span><span class="sxs-lookup"><span data-stu-id="5f810-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> <span data-ttu-id="5f810-121">**注意**</span><span class="sxs-lookup"><span data-stu-id="5f810-121">**Note**</span></span> 
> 
> - <span data-ttu-id="5f810-122">_标识_ 是指创建策略时的策略名称，但在授予策略时是指用户 ID。</span><span class="sxs-lookup"><span data-stu-id="5f810-122">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="5f810-123">对应用程序访问策略的更改最多可能需要 30 分钟才能在 Microsoft Graph REST API 调用中生效。</span><span class="sxs-lookup"><span data-stu-id="5f810-123">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="5f810-124">受支持的权限和其他资源</span><span class="sxs-lookup"><span data-stu-id="5f810-124">Supported permissions and additional resources</span></span>

<span data-ttu-id="5f810-125">管理员可以使用 ApplicationAccessPolicy cmdlet 控制已被授予以下任何应用程序权限的应用的邮箱访问权限：</span><span class="sxs-lookup"><span data-stu-id="5f810-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="5f810-126">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f810-126">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="5f810-127">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f810-127">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="5f810-128">有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/skype/new-csapplicationaccesspolicy)。</span><span class="sxs-lookup"><span data-stu-id="5f810-128">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="5f810-129">错误</span><span class="sxs-lookup"><span data-stu-id="5f810-129">Errors</span></span>

<span data-ttu-id="5f810-130">当 API 调用由于应用在未配置应用程序访问策略时尝试访问联机会议而被拒绝访问时，可能会遇到以下错误。</span><span class="sxs-lookup"><span data-stu-id="5f810-130">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

```json
{
    "error": {
        "code": "Unauthorized",
        "message": "App <app_ID_redacted> is not authorized to Create meeting on behalf of user <user_ID_redacted>",
        "innerError": {
            "date": "<date_redacted>",
            "request-id": "599d9cb0-56ac-4dc5-b6f8-1456a1414609"
        }
    }
}
```

<span data-ttu-id="5f810-131">按照本文中的步骤创建和/或向用户 ID 授予包含应用 ID 的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="5f810-131">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="5f810-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5f810-132">See also</span></span>

- [<span data-ttu-id="5f810-133">权限参考</span><span class="sxs-lookup"><span data-stu-id="5f810-133">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="5f810-134">New-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5f810-134">New-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="5f810-135">Grant-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5f810-135">Grant-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="5f810-136">Get-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5f810-136">Get-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="5f810-137">Set-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5f810-137">Set-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="5f810-138">Remove-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5f810-138">Remove-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
