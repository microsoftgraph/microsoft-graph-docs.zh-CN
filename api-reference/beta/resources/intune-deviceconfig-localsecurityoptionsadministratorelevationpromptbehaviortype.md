---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d0d5c8cd8a38589cef548d03c290015bd4368e12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439860"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="4387b-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4387b-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="4387b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4387b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4387b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4387b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4387b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4387b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4387b-107">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="4387b-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="4387b-108">成员</span><span class="sxs-lookup"><span data-stu-id="4387b-108">Members</span></span>
|<span data-ttu-id="4387b-109">成员</span><span class="sxs-lookup"><span data-stu-id="4387b-109">Member</span></span>|<span data-ttu-id="4387b-110">值</span><span class="sxs-lookup"><span data-stu-id="4387b-110">Value</span></span>|<span data-ttu-id="4387b-111">说明</span><span class="sxs-lookup"><span data-stu-id="4387b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4387b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4387b-112">notConfigured</span></span>|<span data-ttu-id="4387b-113">0</span><span class="sxs-lookup"><span data-stu-id="4387b-113">0</span></span>|<span data-ttu-id="4387b-114">未配置</span><span class="sxs-lookup"><span data-stu-id="4387b-114">Not Configured</span></span>|
|<span data-ttu-id="4387b-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="4387b-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="4387b-116">1</span><span class="sxs-lookup"><span data-stu-id="4387b-116">1</span></span>|<span data-ttu-id="4387b-117">在不提示的情况下提升。</span><span class="sxs-lookup"><span data-stu-id="4387b-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="4387b-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4387b-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="4387b-119">双面</span><span class="sxs-lookup"><span data-stu-id="4387b-119">2</span></span>|<span data-ttu-id="4387b-120">在安全桌面上提示凭据</span><span class="sxs-lookup"><span data-stu-id="4387b-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="4387b-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4387b-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="4387b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="4387b-122">3</span></span>|<span data-ttu-id="4387b-123">安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="4387b-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="4387b-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="4387b-124">promptForCredentials</span></span>|<span data-ttu-id="4387b-125">4 </span><span class="sxs-lookup"><span data-stu-id="4387b-125">4</span></span>|<span data-ttu-id="4387b-126">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="4387b-126">Prompt for credentials</span></span>|
|<span data-ttu-id="4387b-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="4387b-127">promptForConsent</span></span>|<span data-ttu-id="4387b-128">5 </span><span class="sxs-lookup"><span data-stu-id="4387b-128">5</span></span>|<span data-ttu-id="4387b-129">同意提示</span><span class="sxs-lookup"><span data-stu-id="4387b-129">Prompt for consent</span></span>|
|<span data-ttu-id="4387b-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="4387b-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="4387b-131">6 </span><span class="sxs-lookup"><span data-stu-id="4387b-131">6</span></span>|<span data-ttu-id="4387b-132">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="4387b-132">Prompt for consent for non-Windows binaries</span></span>|



