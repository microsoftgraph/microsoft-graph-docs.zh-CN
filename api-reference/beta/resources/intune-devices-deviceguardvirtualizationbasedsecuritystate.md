---
title: deviceGuardVirtualizationBasedSecurityState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01b8c11e12e1a219db8d64dd9f1734b7227df6bd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43362405"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="34c51-103">deviceGuardVirtualizationBasedSecurityState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="34c51-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

<span data-ttu-id="34c51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34c51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34c51-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34c51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34c51-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34c51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34c51-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34c51-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="34c51-108">成员</span><span class="sxs-lookup"><span data-stu-id="34c51-108">Members</span></span>
|<span data-ttu-id="34c51-109">成员</span><span class="sxs-lookup"><span data-stu-id="34c51-109">Member</span></span>|<span data-ttu-id="34c51-110">值</span><span class="sxs-lookup"><span data-stu-id="34c51-110">Value</span></span>|<span data-ttu-id="34c51-111">说明</span><span class="sxs-lookup"><span data-stu-id="34c51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c51-112">运行</span><span class="sxs-lookup"><span data-stu-id="34c51-112">running</span></span>|<span data-ttu-id="34c51-113">0</span><span class="sxs-lookup"><span data-stu-id="34c51-113">0</span></span>|<span data-ttu-id="34c51-114">正在运行</span><span class="sxs-lookup"><span data-stu-id="34c51-114">Running</span></span>|
|<span data-ttu-id="34c51-115">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="34c51-115">rebootRequired</span></span>|<span data-ttu-id="34c51-116">1</span><span class="sxs-lookup"><span data-stu-id="34c51-116">1</span></span>|<span data-ttu-id="34c51-117">根必需</span><span class="sxs-lookup"><span data-stu-id="34c51-117">Root required</span></span>|
|<span data-ttu-id="34c51-118">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="34c51-118">require64BitArchitecture</span></span>|<span data-ttu-id="34c51-119">双面</span><span class="sxs-lookup"><span data-stu-id="34c51-119">2</span></span>|<span data-ttu-id="34c51-120">需要64位体系结构</span><span class="sxs-lookup"><span data-stu-id="34c51-120">64 bit architecture required</span></span>|
|<span data-ttu-id="34c51-121">notLicensed</span><span class="sxs-lookup"><span data-stu-id="34c51-121">notLicensed</span></span>|<span data-ttu-id="34c51-122">第三章</span><span class="sxs-lookup"><span data-stu-id="34c51-122">3</span></span>|<span data-ttu-id="34c51-123">未许可</span><span class="sxs-lookup"><span data-stu-id="34c51-123">Not licensed</span></span>|
|<span data-ttu-id="34c51-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="34c51-124">notConfigured</span></span>|<span data-ttu-id="34c51-125">4 </span><span class="sxs-lookup"><span data-stu-id="34c51-125">4</span></span>|<span data-ttu-id="34c51-126">未配置</span><span class="sxs-lookup"><span data-stu-id="34c51-126">Not configured</span></span>|
|<span data-ttu-id="34c51-127">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="34c51-127">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="34c51-128">5 </span><span class="sxs-lookup"><span data-stu-id="34c51-128">5</span></span>|<span data-ttu-id="34c51-129">系统不满足硬件要求</span><span class="sxs-lookup"><span data-stu-id="34c51-129">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="34c51-130">相互</span><span class="sxs-lookup"><span data-stu-id="34c51-130">other</span></span>|<span data-ttu-id="34c51-131">42</span><span class="sxs-lookup"><span data-stu-id="34c51-131">42</span></span>|<span data-ttu-id="34c51-132">相互.</span><span class="sxs-lookup"><span data-stu-id="34c51-132">Other.</span></span> <span data-ttu-id="34c51-133">Microsoft-DeviceGuard 中的事件日志包含更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="34c51-133">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|



