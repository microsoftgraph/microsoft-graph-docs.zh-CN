---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5039fca8b3cc90e1fd87f0ff11a23685e880985
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946033"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="4eebc-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4eebc-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="4eebc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4eebc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eebc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eebc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eebc-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="4eebc-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="4eebc-107">成员</span><span class="sxs-lookup"><span data-stu-id="4eebc-107">Members</span></span>
|<span data-ttu-id="4eebc-108">成员</span><span class="sxs-lookup"><span data-stu-id="4eebc-108">Member</span></span>|<span data-ttu-id="4eebc-109">值</span><span class="sxs-lookup"><span data-stu-id="4eebc-109">Value</span></span>|<span data-ttu-id="4eebc-110">说明</span><span class="sxs-lookup"><span data-stu-id="4eebc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eebc-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4eebc-111">notConfigured</span></span>|<span data-ttu-id="4eebc-112">0</span><span class="sxs-lookup"><span data-stu-id="4eebc-112">0</span></span>|<span data-ttu-id="4eebc-113">未配置</span><span class="sxs-lookup"><span data-stu-id="4eebc-113">Not Configured</span></span>|
|<span data-ttu-id="4eebc-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="4eebc-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="4eebc-115">1</span><span class="sxs-lookup"><span data-stu-id="4eebc-115">1</span></span>|<span data-ttu-id="4eebc-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="4eebc-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="4eebc-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4eebc-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="4eebc-118">双面</span><span class="sxs-lookup"><span data-stu-id="4eebc-118">2</span></span>|<span data-ttu-id="4eebc-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="4eebc-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="4eebc-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4eebc-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="4eebc-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4eebc-121">3</span></span>|<span data-ttu-id="4eebc-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="4eebc-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="4eebc-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="4eebc-123">promptForCredentials</span></span>|<span data-ttu-id="4eebc-124">4</span><span class="sxs-lookup"><span data-stu-id="4eebc-124">4</span></span>|<span data-ttu-id="4eebc-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="4eebc-125">Prompt for credentials</span></span>|
|<span data-ttu-id="4eebc-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="4eebc-126">promptForConsent</span></span>|<span data-ttu-id="4eebc-127">5</span><span class="sxs-lookup"><span data-stu-id="4eebc-127">5</span></span>|<span data-ttu-id="4eebc-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="4eebc-128">Prompt for consent</span></span>|
|<span data-ttu-id="4eebc-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="4eebc-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="4eebc-130">型</span><span class="sxs-lookup"><span data-stu-id="4eebc-130">6</span></span>|<span data-ttu-id="4eebc-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="4eebc-131">Prompt for consent for non-Windows binaries</span></span>|




