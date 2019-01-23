---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 978436bca4ac0ca281fde61e046e854ba3725c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413757"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="2cc75-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2cc75-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="2cc75-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2cc75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cc75-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2cc75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cc75-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cc75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc75-107">LocalSecurityOptionsAdministratorElevationPromptBehavior 的可能值</span><span class="sxs-lookup"><span data-stu-id="2cc75-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="2cc75-108">成员</span><span class="sxs-lookup"><span data-stu-id="2cc75-108">Members</span></span>
|<span data-ttu-id="2cc75-109">成员</span><span class="sxs-lookup"><span data-stu-id="2cc75-109">Member</span></span>|<span data-ttu-id="2cc75-110">值</span><span class="sxs-lookup"><span data-stu-id="2cc75-110">Value</span></span>|<span data-ttu-id="2cc75-111">说明</span><span class="sxs-lookup"><span data-stu-id="2cc75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc75-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2cc75-112">notConfigured</span></span>|<span data-ttu-id="2cc75-113">0</span><span class="sxs-lookup"><span data-stu-id="2cc75-113">0</span></span>|<span data-ttu-id="2cc75-114">未配置</span><span class="sxs-lookup"><span data-stu-id="2cc75-114">Not Configured</span></span>|
|<span data-ttu-id="2cc75-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="2cc75-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="2cc75-116">1</span><span class="sxs-lookup"><span data-stu-id="2cc75-116">1</span></span>|<span data-ttu-id="2cc75-117">无提示提升。</span><span class="sxs-lookup"><span data-stu-id="2cc75-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="2cc75-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="2cc75-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="2cc75-119">2</span><span class="sxs-lookup"><span data-stu-id="2cc75-119">2</span></span>|<span data-ttu-id="2cc75-120">在安全桌面上的凭据的提示</span><span class="sxs-lookup"><span data-stu-id="2cc75-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="2cc75-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="2cc75-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="2cc75-122">3</span><span class="sxs-lookup"><span data-stu-id="2cc75-122">3</span></span>|<span data-ttu-id="2cc75-123">在安全桌面上的同意提示</span><span class="sxs-lookup"><span data-stu-id="2cc75-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="2cc75-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="2cc75-124">promptForCredentials</span></span>|<span data-ttu-id="2cc75-125">4</span><span class="sxs-lookup"><span data-stu-id="2cc75-125">4</span></span>|<span data-ttu-id="2cc75-126">提示输入凭据</span><span class="sxs-lookup"><span data-stu-id="2cc75-126">Prompt for credentials</span></span>|
|<span data-ttu-id="2cc75-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="2cc75-127">promptForConsent</span></span>|<span data-ttu-id="2cc75-128">5</span><span class="sxs-lookup"><span data-stu-id="2cc75-128">5</span></span>|<span data-ttu-id="2cc75-129">同意提示</span><span class="sxs-lookup"><span data-stu-id="2cc75-129">Prompt for consent</span></span>|
|<span data-ttu-id="2cc75-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="2cc75-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="2cc75-131">6</span><span class="sxs-lookup"><span data-stu-id="2cc75-131">6</span></span>|<span data-ttu-id="2cc75-132">非 Windows 二进制文件的同意提示</span><span class="sxs-lookup"><span data-stu-id="2cc75-132">Prompt for consent for non-Windows binaries</span></span>|




