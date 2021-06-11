---
title: 允许应用程序代表用户访问联机会议
description: 了解如何配置应用程序以代表用户访问联机会议。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: fa3771c1325f0c2a5f10b425e2eca51e9d1534ac
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896702"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="2978f-103">允许应用程序代表用户访问联机会议</span><span class="sxs-lookup"><span data-stu-id="2978f-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="2978f-104">在某些情况下，例如对于在服务器上运行的后台服务或守护程序应用，在没有登录用户的情况下运行，应用可以调用 Microsoft Graph 代表用户采取措施。</span><span class="sxs-lookup"><span data-stu-id="2978f-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="2978f-105">例如，应用可能需要致电 Microsoft Graph，根据发布的计划（如课程 (或外部计划) 安排多个会议。</span><span class="sxs-lookup"><span data-stu-id="2978f-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="2978f-106">在这些情况下，应用程序代表的用户将被标识为会议组织者。</span><span class="sxs-lookup"><span data-stu-id="2978f-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="2978f-107">希望允许应用程序代表用户访问联机会议资源的管理员可以使用 **New-CsApplicationAccessPolicy** 和 **Grant-CsApplicationAccessPolicy** PowerShell cmdlet 配置访问控制。</span><span class="sxs-lookup"><span data-stu-id="2978f-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="2978f-108">本文介绍了配置应用程序访问策略的基本步骤。</span><span class="sxs-lookup"><span data-stu-id="2978f-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="2978f-109">这些步骤特定于联机会议，不适用于其他 Microsoft Graph资源。</span><span class="sxs-lookup"><span data-stu-id="2978f-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="2978f-110">配置应用程序访问策略</span><span class="sxs-lookup"><span data-stu-id="2978f-110">Configure application access policy</span></span>

<span data-ttu-id="2978f-111">要配置应用程序访问策略并允许应用程序访问具有应用程序权限的联机会议，请执行：</span><span class="sxs-lookup"><span data-stu-id="2978f-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="2978f-112">标识应用的应用程序 (客户端) ID 以及将授权应用访问联机会议的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2978f-112">Identify the app’s application (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="2978f-113">在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。</span><span class="sxs-lookup"><span data-stu-id="2978f-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="2978f-114">在 Azure 用户管理门户 (用户) 标识 [用户对象 ID](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="2978f-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="2978f-115">连接管理员Skype for Business PowerShell。</span><span class="sxs-lookup"><span data-stu-id="2978f-115">Connect to Skype for Business PowerShell with an administrator account.</span></span> <span data-ttu-id="2978f-116">有关详细信息，请参阅[使用 PowerShell Skype for Business Online。](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="2978f-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="2978f-117">创建包含应用 ID 列表的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="2978f-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="2978f-118">运行以下 cmdlet，将Identity、AppIds 和 **Description** (可选) 参数。 </span><span class="sxs-lookup"><span data-stu-id="2978f-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="2978f-119">向用户授予策略，以允许策略中包含的应用 ID 代表已授予用户访问联机会议。</span><span class="sxs-lookup"><span data-stu-id="2978f-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="2978f-120">运行以下 cmdlet，替换 **PolicyName 和** **Identity** 参数。</span><span class="sxs-lookup"><span data-stu-id="2978f-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> [!NOTE]
> - <span data-ttu-id="2978f-121">_Identity_ 指创建策略时的策略名称，但在授予策略时指用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2978f-121">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="2978f-122">对应用程序访问策略的更改最多可能需要 30 分钟，才能在 Microsoft Graph REST API 调用中生效。</span><span class="sxs-lookup"><span data-stu-id="2978f-122">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="2978f-123">受支持的权限和其他资源</span><span class="sxs-lookup"><span data-stu-id="2978f-123">Supported permissions and additional resources</span></span>

<span data-ttu-id="2978f-124">管理员可以使用 ApplicationAccessPolicy cmdlet 控制已被授予以下任一应用程序权限的应用的邮箱访问权限：</span><span class="sxs-lookup"><span data-stu-id="2978f-124">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="2978f-125">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2978f-125">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="2978f-126">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2978f-126">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="2978f-127">有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/skype/new-csapplicationaccesspolicy)。</span><span class="sxs-lookup"><span data-stu-id="2978f-127">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="2978f-128">错误</span><span class="sxs-lookup"><span data-stu-id="2978f-128">Errors</span></span>

<span data-ttu-id="2978f-129">当 API 调用因应用在未配置应用程序访问策略时尝试访问联机会议而被拒绝访问时，可能会遇到以下错误。</span><span class="sxs-lookup"><span data-stu-id="2978f-129">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

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

<span data-ttu-id="2978f-130">按照本文中的步骤创建和/或向用户 ID 授予包含应用 ID 的应用程序访问策略。</span><span class="sxs-lookup"><span data-stu-id="2978f-130">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="2978f-131">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2978f-131">See also</span></span>

- [<span data-ttu-id="2978f-132">权限参考</span><span class="sxs-lookup"><span data-stu-id="2978f-132">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="2978f-133">New-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2978f-133">New-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="2978f-134">Grant-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2978f-134">Grant-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="2978f-135">Get-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2978f-135">Get-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="2978f-136">Set-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2978f-136">Set-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="2978f-137">Remove-CsApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="2978f-137">Remove-CsApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
