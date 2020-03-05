---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01f4cd1450e98b5c54e90d73af2e9d3278f24447
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529755"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="14a74-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14a74-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="14a74-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="14a74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14a74-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14a74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14a74-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14a74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14a74-107">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="14a74-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="14a74-108">成员</span><span class="sxs-lookup"><span data-stu-id="14a74-108">Members</span></span>
|<span data-ttu-id="14a74-109">成员</span><span class="sxs-lookup"><span data-stu-id="14a74-109">Member</span></span>|<span data-ttu-id="14a74-110">值</span><span class="sxs-lookup"><span data-stu-id="14a74-110">Value</span></span>|<span data-ttu-id="14a74-111">说明</span><span class="sxs-lookup"><span data-stu-id="14a74-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14a74-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="14a74-112">notConfigured</span></span>|<span data-ttu-id="14a74-113">0</span><span class="sxs-lookup"><span data-stu-id="14a74-113">0</span></span>|<span data-ttu-id="14a74-114">未配置</span><span class="sxs-lookup"><span data-stu-id="14a74-114">Not Configured</span></span>|
|<span data-ttu-id="14a74-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="14a74-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="14a74-116">1 </span><span class="sxs-lookup"><span data-stu-id="14a74-116">1</span></span>|<span data-ttu-id="14a74-117">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="14a74-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="14a74-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="14a74-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="14a74-119">2 </span><span class="sxs-lookup"><span data-stu-id="14a74-119">2</span></span>|<span data-ttu-id="14a74-120">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="14a74-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="14a74-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="14a74-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="14a74-122">3 </span><span class="sxs-lookup"><span data-stu-id="14a74-122">3</span></span>|<span data-ttu-id="14a74-123">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="14a74-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="14a74-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="14a74-124">promptForCredentials</span></span>|<span data-ttu-id="14a74-125">4 </span><span class="sxs-lookup"><span data-stu-id="14a74-125">4</span></span>|<span data-ttu-id="14a74-126">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="14a74-126">Prompt for credentials</span></span>|
|<span data-ttu-id="14a74-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="14a74-127">promptForConsent</span></span>|<span data-ttu-id="14a74-128">5 </span><span class="sxs-lookup"><span data-stu-id="14a74-128">5</span></span>|<span data-ttu-id="14a74-129">同意提示</span><span class="sxs-lookup"><span data-stu-id="14a74-129">Prompt for consent</span></span>|
|<span data-ttu-id="14a74-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="14a74-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="14a74-131">6 </span><span class="sxs-lookup"><span data-stu-id="14a74-131">6</span></span>|<span data-ttu-id="14a74-132">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="14a74-132">Prompt for consent for non-Windows binaries</span></span>|



