---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03131e10101cfd582e558b68fc382b075602a069
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790368"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="216c9-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="216c9-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="216c9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="216c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="216c9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="216c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="216c9-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="216c9-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="216c9-107">成员</span><span class="sxs-lookup"><span data-stu-id="216c9-107">Members</span></span>
|<span data-ttu-id="216c9-108">成员</span><span class="sxs-lookup"><span data-stu-id="216c9-108">Member</span></span>|<span data-ttu-id="216c9-109">值</span><span class="sxs-lookup"><span data-stu-id="216c9-109">Value</span></span>|<span data-ttu-id="216c9-110">说明</span><span class="sxs-lookup"><span data-stu-id="216c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="216c9-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="216c9-111">notConfigured</span></span>|<span data-ttu-id="216c9-112">0</span><span class="sxs-lookup"><span data-stu-id="216c9-112">0</span></span>|<span data-ttu-id="216c9-113">未配置</span><span class="sxs-lookup"><span data-stu-id="216c9-113">Not Configured</span></span>|
|<span data-ttu-id="216c9-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="216c9-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="216c9-115">1</span><span class="sxs-lookup"><span data-stu-id="216c9-115">1</span></span>|<span data-ttu-id="216c9-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="216c9-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="216c9-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="216c9-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="216c9-118">双面</span><span class="sxs-lookup"><span data-stu-id="216c9-118">2</span></span>|<span data-ttu-id="216c9-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="216c9-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="216c9-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="216c9-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="216c9-121">第三章</span><span class="sxs-lookup"><span data-stu-id="216c9-121">3</span></span>|<span data-ttu-id="216c9-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="216c9-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="216c9-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="216c9-123">promptForCredentials</span></span>|<span data-ttu-id="216c9-124">4 </span><span class="sxs-lookup"><span data-stu-id="216c9-124">4</span></span>|<span data-ttu-id="216c9-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="216c9-125">Prompt for credentials</span></span>|
|<span data-ttu-id="216c9-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="216c9-126">promptForConsent</span></span>|<span data-ttu-id="216c9-127">5 </span><span class="sxs-lookup"><span data-stu-id="216c9-127">5</span></span>|<span data-ttu-id="216c9-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="216c9-128">Prompt for consent</span></span>|
|<span data-ttu-id="216c9-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="216c9-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="216c9-130">6 </span><span class="sxs-lookup"><span data-stu-id="216c9-130">6</span></span>|<span data-ttu-id="216c9-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="216c9-131">Prompt for consent for non-Windows binaries</span></span>|



