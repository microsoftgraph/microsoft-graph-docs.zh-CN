---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
ms.openlocfilehash: 2959aebbb12bc567427c8a9b06a5ce2380933241
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044929"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="17d77-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="17d77-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="17d77-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="17d77-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17d77-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17d77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17d77-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="17d77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17d77-107">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="17d77-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="17d77-108">成员</span><span class="sxs-lookup"><span data-stu-id="17d77-108">Members</span></span>
|<span data-ttu-id="17d77-109">成员</span><span class="sxs-lookup"><span data-stu-id="17d77-109">Member</span></span>|<span data-ttu-id="17d77-110">值</span><span class="sxs-lookup"><span data-stu-id="17d77-110">Value</span></span>|<span data-ttu-id="17d77-111">说明</span><span class="sxs-lookup"><span data-stu-id="17d77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17d77-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="17d77-112">notConfigured</span></span>|<span data-ttu-id="17d77-113">0</span><span class="sxs-lookup"><span data-stu-id="17d77-113">0</span></span>|<span data-ttu-id="17d77-114">未配置</span><span class="sxs-lookup"><span data-stu-id="17d77-114">Not Configured</span></span>|
|<span data-ttu-id="17d77-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="17d77-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="17d77-116">1</span><span class="sxs-lookup"><span data-stu-id="17d77-116">1</span></span>|<span data-ttu-id="17d77-117">无提示提升。</span><span class="sxs-lookup"><span data-stu-id="17d77-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="17d77-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="17d77-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="17d77-119">2</span><span class="sxs-lookup"><span data-stu-id="17d77-119">2</span></span>|<span data-ttu-id="17d77-120">在安全桌面上的凭据的提示</span><span class="sxs-lookup"><span data-stu-id="17d77-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="17d77-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="17d77-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="17d77-122">3</span><span class="sxs-lookup"><span data-stu-id="17d77-122">3</span></span>|<span data-ttu-id="17d77-123">在安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="17d77-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="17d77-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="17d77-124">promptForCredentials</span></span>|<span data-ttu-id="17d77-125">4</span><span class="sxs-lookup"><span data-stu-id="17d77-125">4</span></span>|<span data-ttu-id="17d77-126">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="17d77-126">Prompt for credentials</span></span>|
|<span data-ttu-id="17d77-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="17d77-127">promptForConsent</span></span>|<span data-ttu-id="17d77-128">5</span><span class="sxs-lookup"><span data-stu-id="17d77-128">5</span></span>|<span data-ttu-id="17d77-129">同意提示</span><span class="sxs-lookup"><span data-stu-id="17d77-129">Prompt for consent</span></span>|
|<span data-ttu-id="17d77-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="17d77-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="17d77-131">6</span><span class="sxs-lookup"><span data-stu-id="17d77-131">6</span></span>|<span data-ttu-id="17d77-132">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="17d77-132">Prompt for consent for non-Windows binaries</span></span>|





