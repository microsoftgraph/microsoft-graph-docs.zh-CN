---
title: 允许 applicatiosn 代表用户访问在线会议
description: 了解如何配置应用程序以代表用户访问在线会议。
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: fc96bd7958fd2729c9222bdb88b50fb04608732a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289461"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="43533-103">允许应用程序代表用户访问在线会议</span><span class="sxs-lookup"><span data-stu-id="43533-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="43533-104">在某些情况下，例如，对于在不存在登录用户的服务器上运行的后台服务或守护程序应用程序，应用程序可以调用 Microsoft Graph 以代表用户执行操作。</span><span class="sxs-lookup"><span data-stu-id="43533-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="43533-105">例如，应用可能需要调用 Microsoft Graph，以根据发布的日程安排多个会议 (例如课程) 或外部计划工具。</span><span class="sxs-lookup"><span data-stu-id="43533-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="43533-106">在这些情况下，应用程序代表的用户标识为会议组织者。</span><span class="sxs-lookup"><span data-stu-id="43533-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="43533-107">希望允许应用程序代表用户访问联机会议资源的管理员可以使用 **CsApplicationAccessPolicy** 和 **CsApplicationAccessPolicy** PowerShell cmdlet 配置访问控制。</span><span class="sxs-lookup"><span data-stu-id="43533-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="43533-108">本文介绍了配置应用程序访问策略的基本步骤。</span><span class="sxs-lookup"><span data-stu-id="43533-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="43533-109">这些步骤特定于联机会议，不应用于其他 Microsoft Graph 资源。</span><span class="sxs-lookup"><span data-stu-id="43533-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="43533-110">配置应用程序访问策略</span><span class="sxs-lookup"><span data-stu-id="43533-110">Configure application access policy</span></span>

<span data-ttu-id="43533-111">若要配置应用程序访问策略并允许应用程序使用应用程序权限访问联机会议，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="43533-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="43533-112">标识应用程序的 applcation (客户端) ID 和代表用户的用户 Id，该应用程序将被授权访问联机会议。</span><span class="sxs-lookup"><span data-stu-id="43533-112">Identify the app’s applcation (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="43533-113">在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。</span><span class="sxs-lookup"><span data-stu-id="43533-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="43533-114">在[Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中标识用户的用户 (对象) ID</span><span class="sxs-lookup"><span data-stu-id="43533-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="43533-115">使用 adminitrator 帐户连接到 Skype for Business PowerShell。</span><span class="sxs-lookup"><span data-stu-id="43533-115">Connect to Skype for Business PowerShell with adminitrator account.</span></span> <span data-ttu-id="43533-116">有关详细信息，请参阅 [使用 PowerShell 管理 Skype For Business Online](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)。</span><span class="sxs-lookup"><span data-stu-id="43533-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="43533-117">创建包含应用程序 Id 列表的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="43533-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="43533-118">运行以下 cmdlet，将 **Identity**、 **AppIds**和 **Description** 替换 (可选的) 参数。</span><span class="sxs-lookup"><span data-stu-id="43533-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="43533-119">向用户授予策略，以便允许包含在策略中的应用程序 Id 代表授予用户访问联机会议。</span><span class="sxs-lookup"><span data-stu-id="43533-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="43533-120">运行以下 cmdlet 以替换 **PolicyName** 和 **Identity** 参数。</span><span class="sxs-lookup"><span data-stu-id="43533-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> <span data-ttu-id="43533-121">**注意**</span><span class="sxs-lookup"><span data-stu-id="43533-121">**Note**</span></span> 
> 
> - <span data-ttu-id="43533-122">_标识_ 是指创建策略时的策略名称，但在授予策略时是用户 ID。</span><span class="sxs-lookup"><span data-stu-id="43533-122">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="43533-123">对应用程序访问策略所做的更改可能需要30分钟才能在 Microsoft Graph REST API 调用中生效。</span><span class="sxs-lookup"><span data-stu-id="43533-123">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="43533-124">受支持的权限和其他资源</span><span class="sxs-lookup"><span data-stu-id="43533-124">Supported permissions and additional resources</span></span>

<span data-ttu-id="43533-125">管理员可以使用 ApplicationAccessPolicy cmdlet 来控制已授予以下任一应用程序权限的应用的邮箱访问权限：</span><span class="sxs-lookup"><span data-stu-id="43533-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="43533-126">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="43533-126">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="43533-127">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43533-127">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="43533-128">有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/skype/new-csapplicationaccesspolicy)。</span><span class="sxs-lookup"><span data-stu-id="43533-128">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="43533-129">错误</span><span class="sxs-lookup"><span data-stu-id="43533-129">Errors</span></span>

<span data-ttu-id="43533-130">如果在未配置应用程序访问策略时试图访问联机会议的应用程序导致 API 调用被拒绝，则可能会遇到以下错误。</span><span class="sxs-lookup"><span data-stu-id="43533-130">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

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

<span data-ttu-id="43533-131">按照本文中的步骤操作，创建和/或将包含应用程序 ID 的应用程序访问策略授予用户 ID。</span><span class="sxs-lookup"><span data-stu-id="43533-131">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="43533-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="43533-132">See also</span></span>

- [<span data-ttu-id="43533-133">权限参考</span><span class="sxs-lookup"><span data-stu-id="43533-133">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="43533-134">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="43533-134">New-ApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="43533-135">Grant-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="43533-135">Grant-ApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="43533-136">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="43533-136">Get-ApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="43533-137">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="43533-137">Set-ApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="43533-138">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="43533-138">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)