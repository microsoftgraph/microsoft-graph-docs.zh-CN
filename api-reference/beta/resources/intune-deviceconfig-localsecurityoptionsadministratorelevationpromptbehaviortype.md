---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796932"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="e8a14-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e8a14-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="e8a14-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8a14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8a14-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8a14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8a14-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="e8a14-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="e8a14-107">成员</span><span class="sxs-lookup"><span data-stu-id="e8a14-107">Members</span></span>
|<span data-ttu-id="e8a14-108">成员</span><span class="sxs-lookup"><span data-stu-id="e8a14-108">Member</span></span>|<span data-ttu-id="e8a14-109">值</span><span class="sxs-lookup"><span data-stu-id="e8a14-109">Value</span></span>|<span data-ttu-id="e8a14-110">说明</span><span class="sxs-lookup"><span data-stu-id="e8a14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8a14-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e8a14-111">notConfigured</span></span>|<span data-ttu-id="e8a14-112">0</span><span class="sxs-lookup"><span data-stu-id="e8a14-112">0</span></span>|<span data-ttu-id="e8a14-113">未配置</span><span class="sxs-lookup"><span data-stu-id="e8a14-113">Not Configured</span></span>|
|<span data-ttu-id="e8a14-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="e8a14-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="e8a14-115">1</span><span class="sxs-lookup"><span data-stu-id="e8a14-115">1</span></span>|<span data-ttu-id="e8a14-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="e8a14-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="e8a14-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="e8a14-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="e8a14-118">双面</span><span class="sxs-lookup"><span data-stu-id="e8a14-118">2</span></span>|<span data-ttu-id="e8a14-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="e8a14-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="e8a14-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="e8a14-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="e8a14-121">第三章</span><span class="sxs-lookup"><span data-stu-id="e8a14-121">3</span></span>|<span data-ttu-id="e8a14-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="e8a14-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="e8a14-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="e8a14-123">promptForCredentials</span></span>|<span data-ttu-id="e8a14-124">4</span><span class="sxs-lookup"><span data-stu-id="e8a14-124">4</span></span>|<span data-ttu-id="e8a14-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="e8a14-125">Prompt for credentials</span></span>|
|<span data-ttu-id="e8a14-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="e8a14-126">promptForConsent</span></span>|<span data-ttu-id="e8a14-127">5</span><span class="sxs-lookup"><span data-stu-id="e8a14-127">5</span></span>|<span data-ttu-id="e8a14-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="e8a14-128">Prompt for consent</span></span>|
|<span data-ttu-id="e8a14-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="e8a14-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="e8a14-130">型</span><span class="sxs-lookup"><span data-stu-id="e8a14-130">6</span></span>|<span data-ttu-id="e8a14-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="e8a14-131">Prompt for consent for non-Windows binaries</span></span>|





