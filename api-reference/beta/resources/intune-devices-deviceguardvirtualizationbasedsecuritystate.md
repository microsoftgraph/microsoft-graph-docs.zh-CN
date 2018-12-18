---
title: deviceGuardVirtualizationBasedSecurityState 枚举类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 2d40293a16fb3d424fed38cead82cfd7177df890
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354234"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="717a2-103">deviceGuardVirtualizationBasedSecurityState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="717a2-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="717a2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="717a2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="717a2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="717a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="717a2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="717a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="717a2-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="717a2-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="717a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="717a2-108">Members</span></span>
|<span data-ttu-id="717a2-109">成员</span><span class="sxs-lookup"><span data-stu-id="717a2-109">Member</span></span>|<span data-ttu-id="717a2-110">值</span><span class="sxs-lookup"><span data-stu-id="717a2-110">Value</span></span>|<span data-ttu-id="717a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="717a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="717a2-112">运行</span><span class="sxs-lookup"><span data-stu-id="717a2-112">running</span></span>|<span data-ttu-id="717a2-113">0</span><span class="sxs-lookup"><span data-stu-id="717a2-113">0</span></span>|<span data-ttu-id="717a2-114">运行</span><span class="sxs-lookup"><span data-stu-id="717a2-114">Running</span></span>|
|<span data-ttu-id="717a2-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="717a2-115">rebootRequired</span></span>|<span data-ttu-id="717a2-116">1</span><span class="sxs-lookup"><span data-stu-id="717a2-116">1</span></span>|<span data-ttu-id="717a2-117">所需的根</span><span class="sxs-lookup"><span data-stu-id="717a2-117">Root required</span></span>|
|<span data-ttu-id="717a2-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="717a2-118">require64BitArchitecture</span></span>|<span data-ttu-id="717a2-119">2</span><span class="sxs-lookup"><span data-stu-id="717a2-119">2</span></span>|<span data-ttu-id="717a2-120">所需的 64 位体系结构</span><span class="sxs-lookup"><span data-stu-id="717a2-120">64 bit architecture required</span></span>|
|<span data-ttu-id="717a2-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="717a2-121">notLicensed</span></span>|<span data-ttu-id="717a2-122">3</span><span class="sxs-lookup"><span data-stu-id="717a2-122">3</span></span>|<span data-ttu-id="717a2-123">未授权</span><span class="sxs-lookup"><span data-stu-id="717a2-123">Not licensed</span></span>|
|<span data-ttu-id="717a2-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="717a2-124">notConfigured</span></span>|<span data-ttu-id="717a2-125">4</span><span class="sxs-lookup"><span data-stu-id="717a2-125">4</span></span>|<span data-ttu-id="717a2-126">未配置</span><span class="sxs-lookup"><span data-stu-id="717a2-126">Not configured</span></span>|
|<span data-ttu-id="717a2-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="717a2-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="717a2-128">5</span><span class="sxs-lookup"><span data-stu-id="717a2-128">5</span></span>|<span data-ttu-id="717a2-129">系统不满足硬件要求</span><span class="sxs-lookup"><span data-stu-id="717a2-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="717a2-130">其他</span><span class="sxs-lookup"><span data-stu-id="717a2-130">other</span></span>|<span data-ttu-id="717a2-131">42</span><span class="sxs-lookup"><span data-stu-id="717a2-131">42</span></span>|<span data-ttu-id="717a2-132">其他。</span><span class="sxs-lookup"><span data-stu-id="717a2-132">Other.</span></span> <span data-ttu-id="717a2-133">Microsoft 的 Windows DeviceGuard 中的事件日志具有更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="717a2-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





