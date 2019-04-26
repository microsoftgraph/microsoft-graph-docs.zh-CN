---
title: deviceGuardVirtualizationBasedSecurityState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51def159e90b256e772138264139f2a96fbd3344
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570129"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="7cdc6-103">deviceGuardVirtualizationBasedSecurityState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7cdc6-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="7cdc6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7cdc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cdc6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7cdc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cdc6-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7cdc6-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="7cdc6-107">成员</span><span class="sxs-lookup"><span data-stu-id="7cdc6-107">Members</span></span>
|<span data-ttu-id="7cdc6-108">成员</span><span class="sxs-lookup"><span data-stu-id="7cdc6-108">Member</span></span>|<span data-ttu-id="7cdc6-109">值</span><span class="sxs-lookup"><span data-stu-id="7cdc6-109">Value</span></span>|<span data-ttu-id="7cdc6-110">说明</span><span class="sxs-lookup"><span data-stu-id="7cdc6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cdc6-111">运行</span><span class="sxs-lookup"><span data-stu-id="7cdc6-111">running</span></span>|<span data-ttu-id="7cdc6-112">0</span><span class="sxs-lookup"><span data-stu-id="7cdc6-112">0</span></span>|<span data-ttu-id="7cdc6-113">运行</span><span class="sxs-lookup"><span data-stu-id="7cdc6-113">Running</span></span>|
|<span data-ttu-id="7cdc6-114">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="7cdc6-114">rebootRequired</span></span>|<span data-ttu-id="7cdc6-115">1</span><span class="sxs-lookup"><span data-stu-id="7cdc6-115">1</span></span>|<span data-ttu-id="7cdc6-116">根必需</span><span class="sxs-lookup"><span data-stu-id="7cdc6-116">Root required</span></span>|
|<span data-ttu-id="7cdc6-117">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="7cdc6-117">require64BitArchitecture</span></span>|<span data-ttu-id="7cdc6-118">2 </span><span class="sxs-lookup"><span data-stu-id="7cdc6-118">2</span></span>|<span data-ttu-id="7cdc6-119">需要64位体系结构</span><span class="sxs-lookup"><span data-stu-id="7cdc6-119">64 bit architecture required</span></span>|
|<span data-ttu-id="7cdc6-120">notLicensed</span><span class="sxs-lookup"><span data-stu-id="7cdc6-120">notLicensed</span></span>|<span data-ttu-id="7cdc6-121">3 </span><span class="sxs-lookup"><span data-stu-id="7cdc6-121">3</span></span>|<span data-ttu-id="7cdc6-122">未许可</span><span class="sxs-lookup"><span data-stu-id="7cdc6-122">Not licensed</span></span>|
|<span data-ttu-id="7cdc6-123">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7cdc6-123">notConfigured</span></span>|<span data-ttu-id="7cdc6-124">4 </span><span class="sxs-lookup"><span data-stu-id="7cdc6-124">4</span></span>|<span data-ttu-id="7cdc6-125">未配置</span><span class="sxs-lookup"><span data-stu-id="7cdc6-125">Not configured</span></span>|
|<span data-ttu-id="7cdc6-126">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="7cdc6-126">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="7cdc6-127">5 </span><span class="sxs-lookup"><span data-stu-id="7cdc6-127">5</span></span>|<span data-ttu-id="7cdc6-128">系统不满足硬件要求</span><span class="sxs-lookup"><span data-stu-id="7cdc6-128">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="7cdc6-129">相互</span><span class="sxs-lookup"><span data-stu-id="7cdc6-129">other</span></span>|<span data-ttu-id="7cdc6-130">42</span><span class="sxs-lookup"><span data-stu-id="7cdc6-130">42</span></span>|<span data-ttu-id="7cdc6-131">相互.</span><span class="sxs-lookup"><span data-stu-id="7cdc6-131">Other.</span></span> <span data-ttu-id="7cdc6-132">microsoft-DeviceGuard 中的事件日志包含更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="7cdc6-132">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





