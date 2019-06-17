---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24434b710a80e8839b95168204a4d68b31c20b4c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989355"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="1b098-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b098-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="1b098-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b098-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b098-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b098-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b098-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="1b098-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="1b098-107">成员</span><span class="sxs-lookup"><span data-stu-id="1b098-107">Members</span></span>
|<span data-ttu-id="1b098-108">成员</span><span class="sxs-lookup"><span data-stu-id="1b098-108">Member</span></span>|<span data-ttu-id="1b098-109">值</span><span class="sxs-lookup"><span data-stu-id="1b098-109">Value</span></span>|<span data-ttu-id="1b098-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b098-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b098-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1b098-111">notConfigured</span></span>|<span data-ttu-id="1b098-112">0</span><span class="sxs-lookup"><span data-stu-id="1b098-112">0</span></span>|<span data-ttu-id="1b098-113">未配置</span><span class="sxs-lookup"><span data-stu-id="1b098-113">Not Configured</span></span>|
|<span data-ttu-id="1b098-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="1b098-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="1b098-115">1</span><span class="sxs-lookup"><span data-stu-id="1b098-115">1</span></span>|<span data-ttu-id="1b098-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="1b098-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="1b098-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="1b098-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="1b098-118">双面</span><span class="sxs-lookup"><span data-stu-id="1b098-118">2</span></span>|<span data-ttu-id="1b098-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="1b098-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="1b098-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="1b098-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="1b098-121">第三章</span><span class="sxs-lookup"><span data-stu-id="1b098-121">3</span></span>|<span data-ttu-id="1b098-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="1b098-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="1b098-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="1b098-123">promptForCredentials</span></span>|<span data-ttu-id="1b098-124">4</span><span class="sxs-lookup"><span data-stu-id="1b098-124">4</span></span>|<span data-ttu-id="1b098-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="1b098-125">Prompt for credentials</span></span>|
|<span data-ttu-id="1b098-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="1b098-126">promptForConsent</span></span>|<span data-ttu-id="1b098-127">5</span><span class="sxs-lookup"><span data-stu-id="1b098-127">5</span></span>|<span data-ttu-id="1b098-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="1b098-128">Prompt for consent</span></span>|
|<span data-ttu-id="1b098-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="1b098-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="1b098-130">型</span><span class="sxs-lookup"><span data-stu-id="1b098-130">6</span></span>|<span data-ttu-id="1b098-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="1b098-131">Prompt for consent for non-Windows binaries</span></span>|





