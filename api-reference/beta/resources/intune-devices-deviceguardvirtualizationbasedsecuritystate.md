---
title: deviceGuardVirtualizationBasedSecurityState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2c3d7745af4e6a93e9836f24a184e6ca90b60d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882374"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="11a12-103">deviceGuardVirtualizationBasedSecurityState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11a12-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="11a12-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="11a12-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11a12-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="11a12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11a12-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="11a12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11a12-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="11a12-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="11a12-108">成员</span><span class="sxs-lookup"><span data-stu-id="11a12-108">Members</span></span>
|<span data-ttu-id="11a12-109">成员</span><span class="sxs-lookup"><span data-stu-id="11a12-109">Member</span></span>|<span data-ttu-id="11a12-110">值</span><span class="sxs-lookup"><span data-stu-id="11a12-110">Value</span></span>|<span data-ttu-id="11a12-111">Description</span><span class="sxs-lookup"><span data-stu-id="11a12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11a12-112">运行</span><span class="sxs-lookup"><span data-stu-id="11a12-112">running</span></span>|<span data-ttu-id="11a12-113">0</span><span class="sxs-lookup"><span data-stu-id="11a12-113">0</span></span>|<span data-ttu-id="11a12-114">运行</span><span class="sxs-lookup"><span data-stu-id="11a12-114">Running</span></span>|
|<span data-ttu-id="11a12-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="11a12-115">rebootRequired</span></span>|<span data-ttu-id="11a12-116">1</span><span class="sxs-lookup"><span data-stu-id="11a12-116">1</span></span>|<span data-ttu-id="11a12-117">所需的根</span><span class="sxs-lookup"><span data-stu-id="11a12-117">Root required</span></span>|
|<span data-ttu-id="11a12-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="11a12-118">require64BitArchitecture</span></span>|<span data-ttu-id="11a12-119">2</span><span class="sxs-lookup"><span data-stu-id="11a12-119">2</span></span>|<span data-ttu-id="11a12-120">所需的 64 位体系结构</span><span class="sxs-lookup"><span data-stu-id="11a12-120">64 bit architecture required</span></span>|
|<span data-ttu-id="11a12-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="11a12-121">notLicensed</span></span>|<span data-ttu-id="11a12-122">3</span><span class="sxs-lookup"><span data-stu-id="11a12-122">3</span></span>|<span data-ttu-id="11a12-123">未授权</span><span class="sxs-lookup"><span data-stu-id="11a12-123">Not licensed</span></span>|
|<span data-ttu-id="11a12-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="11a12-124">notConfigured</span></span>|<span data-ttu-id="11a12-125">4</span><span class="sxs-lookup"><span data-stu-id="11a12-125">4</span></span>|<span data-ttu-id="11a12-126">未配置</span><span class="sxs-lookup"><span data-stu-id="11a12-126">Not configured</span></span>|
|<span data-ttu-id="11a12-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="11a12-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="11a12-128">5</span><span class="sxs-lookup"><span data-stu-id="11a12-128">5</span></span>|<span data-ttu-id="11a12-129">系统不满足硬件要求</span><span class="sxs-lookup"><span data-stu-id="11a12-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="11a12-130">其他</span><span class="sxs-lookup"><span data-stu-id="11a12-130">other</span></span>|<span data-ttu-id="11a12-131">42</span><span class="sxs-lookup"><span data-stu-id="11a12-131">42</span></span>|<span data-ttu-id="11a12-132">其他。</span><span class="sxs-lookup"><span data-stu-id="11a12-132">Other.</span></span> <span data-ttu-id="11a12-133">Microsoft 的 Windows DeviceGuard 中的事件日志具有更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="11a12-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





