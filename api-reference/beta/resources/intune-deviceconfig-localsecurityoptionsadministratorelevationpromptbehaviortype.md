---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 424c1193015d688019892d66ed07588358dcb8c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870880"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="c5296-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c5296-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="c5296-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5296-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5296-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5296-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5296-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c5296-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5296-107">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="c5296-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="c5296-108">成员</span><span class="sxs-lookup"><span data-stu-id="c5296-108">Members</span></span>
|<span data-ttu-id="c5296-109">成员</span><span class="sxs-lookup"><span data-stu-id="c5296-109">Member</span></span>|<span data-ttu-id="c5296-110">值</span><span class="sxs-lookup"><span data-stu-id="c5296-110">Value</span></span>|<span data-ttu-id="c5296-111">Description</span><span class="sxs-lookup"><span data-stu-id="c5296-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5296-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c5296-112">notConfigured</span></span>|<span data-ttu-id="c5296-113">0</span><span class="sxs-lookup"><span data-stu-id="c5296-113">0</span></span>|<span data-ttu-id="c5296-114">未配置</span><span class="sxs-lookup"><span data-stu-id="c5296-114">Not Configured</span></span>|
|<span data-ttu-id="c5296-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="c5296-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="c5296-116">1</span><span class="sxs-lookup"><span data-stu-id="c5296-116">1</span></span>|<span data-ttu-id="c5296-117">无提示提升。</span><span class="sxs-lookup"><span data-stu-id="c5296-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="c5296-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="c5296-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="c5296-119">2</span><span class="sxs-lookup"><span data-stu-id="c5296-119">2</span></span>|<span data-ttu-id="c5296-120">在安全桌面上的凭据的提示</span><span class="sxs-lookup"><span data-stu-id="c5296-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="c5296-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="c5296-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="c5296-122">3</span><span class="sxs-lookup"><span data-stu-id="c5296-122">3</span></span>|<span data-ttu-id="c5296-123">在安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="c5296-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="c5296-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="c5296-124">promptForCredentials</span></span>|<span data-ttu-id="c5296-125">4</span><span class="sxs-lookup"><span data-stu-id="c5296-125">4</span></span>|<span data-ttu-id="c5296-126">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="c5296-126">Prompt for credentials</span></span>|
|<span data-ttu-id="c5296-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="c5296-127">promptForConsent</span></span>|<span data-ttu-id="c5296-128">5</span><span class="sxs-lookup"><span data-stu-id="c5296-128">5</span></span>|<span data-ttu-id="c5296-129">同意提示</span><span class="sxs-lookup"><span data-stu-id="c5296-129">Prompt for consent</span></span>|
|<span data-ttu-id="c5296-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="c5296-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="c5296-131">6</span><span class="sxs-lookup"><span data-stu-id="c5296-131">6</span></span>|<span data-ttu-id="c5296-132">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="c5296-132">Prompt for consent for non-Windows binaries</span></span>|





