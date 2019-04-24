---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460525"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="2be68-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2be68-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="2be68-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2be68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2be68-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2be68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2be68-106">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="2be68-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="2be68-107">成员</span><span class="sxs-lookup"><span data-stu-id="2be68-107">Members</span></span>
|<span data-ttu-id="2be68-108">成员</span><span class="sxs-lookup"><span data-stu-id="2be68-108">Member</span></span>|<span data-ttu-id="2be68-109">值</span><span class="sxs-lookup"><span data-stu-id="2be68-109">Value</span></span>|<span data-ttu-id="2be68-110">说明</span><span class="sxs-lookup"><span data-stu-id="2be68-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2be68-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2be68-111">notConfigured</span></span>|<span data-ttu-id="2be68-112">0</span><span class="sxs-lookup"><span data-stu-id="2be68-112">0</span></span>|<span data-ttu-id="2be68-113">未配置</span><span class="sxs-lookup"><span data-stu-id="2be68-113">Not Configured</span></span>|
|<span data-ttu-id="2be68-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="2be68-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="2be68-115">1</span><span class="sxs-lookup"><span data-stu-id="2be68-115">1</span></span>|<span data-ttu-id="2be68-116">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="2be68-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="2be68-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="2be68-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="2be68-118">2 </span><span class="sxs-lookup"><span data-stu-id="2be68-118">2</span></span>|<span data-ttu-id="2be68-119">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="2be68-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="2be68-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="2be68-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="2be68-121">3 </span><span class="sxs-lookup"><span data-stu-id="2be68-121">3</span></span>|<span data-ttu-id="2be68-122">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="2be68-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="2be68-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="2be68-123">promptForCredentials</span></span>|<span data-ttu-id="2be68-124">4 </span><span class="sxs-lookup"><span data-stu-id="2be68-124">4</span></span>|<span data-ttu-id="2be68-125">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="2be68-125">Prompt for credentials</span></span>|
|<span data-ttu-id="2be68-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="2be68-126">promptForConsent</span></span>|<span data-ttu-id="2be68-127">5</span><span class="sxs-lookup"><span data-stu-id="2be68-127">5</span></span>|<span data-ttu-id="2be68-128">同意提示</span><span class="sxs-lookup"><span data-stu-id="2be68-128">Prompt for consent</span></span>|
|<span data-ttu-id="2be68-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="2be68-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="2be68-130">6 </span><span class="sxs-lookup"><span data-stu-id="2be68-130">6</span></span>|<span data-ttu-id="2be68-131">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="2be68-131">Prompt for consent for non-Windows binaries</span></span>|





