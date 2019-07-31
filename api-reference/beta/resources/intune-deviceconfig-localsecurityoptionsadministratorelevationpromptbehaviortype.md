---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 397c8300a6acb2226a5f5dcccf630dde5d31bbc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000996"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="cbd60-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cbd60-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="cbd60-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbd60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbd60-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbd60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbd60-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="cbd60-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="cbd60-107">成员</span><span class="sxs-lookup"><span data-stu-id="cbd60-107">Members</span></span>
|<span data-ttu-id="cbd60-108">成员</span><span class="sxs-lookup"><span data-stu-id="cbd60-108">Member</span></span>|<span data-ttu-id="cbd60-109">值</span><span class="sxs-lookup"><span data-stu-id="cbd60-109">Value</span></span>|<span data-ttu-id="cbd60-110">说明</span><span class="sxs-lookup"><span data-stu-id="cbd60-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd60-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cbd60-111">notConfigured</span></span>|<span data-ttu-id="cbd60-112">0</span><span class="sxs-lookup"><span data-stu-id="cbd60-112">0</span></span>|<span data-ttu-id="cbd60-113">未配置</span><span class="sxs-lookup"><span data-stu-id="cbd60-113">Not Configured</span></span>|
|<span data-ttu-id="cbd60-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="cbd60-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="cbd60-115">1</span><span class="sxs-lookup"><span data-stu-id="cbd60-115">1</span></span>|<span data-ttu-id="cbd60-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="cbd60-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="cbd60-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="cbd60-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="cbd60-118">双面</span><span class="sxs-lookup"><span data-stu-id="cbd60-118">2</span></span>|<span data-ttu-id="cbd60-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="cbd60-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="cbd60-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="cbd60-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="cbd60-121">第三章</span><span class="sxs-lookup"><span data-stu-id="cbd60-121">3</span></span>|<span data-ttu-id="cbd60-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="cbd60-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="cbd60-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="cbd60-123">promptForCredentials</span></span>|<span data-ttu-id="cbd60-124">4</span><span class="sxs-lookup"><span data-stu-id="cbd60-124">4</span></span>|<span data-ttu-id="cbd60-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="cbd60-125">Prompt for credentials</span></span>|
|<span data-ttu-id="cbd60-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="cbd60-126">promptForConsent</span></span>|<span data-ttu-id="cbd60-127">5</span><span class="sxs-lookup"><span data-stu-id="cbd60-127">5</span></span>|<span data-ttu-id="cbd60-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="cbd60-128">Prompt for consent</span></span>|
|<span data-ttu-id="cbd60-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="cbd60-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="cbd60-130">型</span><span class="sxs-lookup"><span data-stu-id="cbd60-130">6</span></span>|<span data-ttu-id="cbd60-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="cbd60-131">Prompt for consent for non-Windows binaries</span></span>|





