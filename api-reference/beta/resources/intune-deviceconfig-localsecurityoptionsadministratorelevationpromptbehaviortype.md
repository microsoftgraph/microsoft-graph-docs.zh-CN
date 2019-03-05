---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5deaccdd8e1f3707617fe2df06a5fec087a47625
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139338"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="daa89-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="daa89-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="daa89-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="daa89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daa89-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="daa89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daa89-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="daa89-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="daa89-107">成员</span><span class="sxs-lookup"><span data-stu-id="daa89-107">Members</span></span>
|<span data-ttu-id="daa89-108">成员</span><span class="sxs-lookup"><span data-stu-id="daa89-108">Member</span></span>|<span data-ttu-id="daa89-109">值</span><span class="sxs-lookup"><span data-stu-id="daa89-109">Value</span></span>|<span data-ttu-id="daa89-110">说明</span><span class="sxs-lookup"><span data-stu-id="daa89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa89-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="daa89-111">notConfigured</span></span>|<span data-ttu-id="daa89-112">0</span><span class="sxs-lookup"><span data-stu-id="daa89-112">0</span></span>|<span data-ttu-id="daa89-113">未配置</span><span class="sxs-lookup"><span data-stu-id="daa89-113">Not Configured</span></span>|
|<span data-ttu-id="daa89-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="daa89-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="daa89-115">1</span><span class="sxs-lookup"><span data-stu-id="daa89-115">1</span></span>|<span data-ttu-id="daa89-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="daa89-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="daa89-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="daa89-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="daa89-118">双面</span><span class="sxs-lookup"><span data-stu-id="daa89-118">2</span></span>|<span data-ttu-id="daa89-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="daa89-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="daa89-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="daa89-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="daa89-121">第三章</span><span class="sxs-lookup"><span data-stu-id="daa89-121">3</span></span>|<span data-ttu-id="daa89-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="daa89-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="daa89-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="daa89-123">promptForCredentials</span></span>|<span data-ttu-id="daa89-124">4</span><span class="sxs-lookup"><span data-stu-id="daa89-124">4</span></span>|<span data-ttu-id="daa89-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="daa89-125">Prompt for credentials</span></span>|
|<span data-ttu-id="daa89-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="daa89-126">promptForConsent</span></span>|<span data-ttu-id="daa89-127">5</span><span class="sxs-lookup"><span data-stu-id="daa89-127">5</span></span>|<span data-ttu-id="daa89-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="daa89-128">Prompt for consent</span></span>|
|<span data-ttu-id="daa89-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="daa89-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="daa89-130">型</span><span class="sxs-lookup"><span data-stu-id="daa89-130">6</span></span>|<span data-ttu-id="daa89-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="daa89-131">Prompt for consent for non-Windows binaries</span></span>|




