---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6086dc05d204e4c9cb23c77f79f98c3a207de35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941889"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="03604-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="03604-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="03604-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03604-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03604-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03604-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03604-106">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="03604-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="03604-107">成员</span><span class="sxs-lookup"><span data-stu-id="03604-107">Members</span></span>
|<span data-ttu-id="03604-108">成员</span><span class="sxs-lookup"><span data-stu-id="03604-108">Member</span></span>|<span data-ttu-id="03604-109">值</span><span class="sxs-lookup"><span data-stu-id="03604-109">Value</span></span>|<span data-ttu-id="03604-110">说明</span><span class="sxs-lookup"><span data-stu-id="03604-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03604-111">清理</span><span class="sxs-lookup"><span data-stu-id="03604-111">clean</span></span>|<span data-ttu-id="03604-112">0</span><span class="sxs-lookup"><span data-stu-id="03604-112">0</span></span>|<span data-ttu-id="03604-113">计算机干净, 无需任何操作</span><span class="sxs-lookup"><span data-stu-id="03604-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="03604-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="03604-114">fullScanPending</span></span>|<span data-ttu-id="03604-115">1</span><span class="sxs-lookup"><span data-stu-id="03604-115">1</span></span>|<span data-ttu-id="03604-116">计算机处于挂起的完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="03604-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="03604-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="03604-117">rebootPending</span></span>|<span data-ttu-id="03604-118">双面</span><span class="sxs-lookup"><span data-stu-id="03604-118">2</span></span>|<span data-ttu-id="03604-119">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="03604-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="03604-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="03604-120">manualStepsPending</span></span>|<span data-ttu-id="03604-121">4</span><span class="sxs-lookup"><span data-stu-id="03604-121">4</span></span>|<span data-ttu-id="03604-122">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="03604-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="03604-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="03604-123">offlineScanPending</span></span>|<span data-ttu-id="03604-124">utf-8</span><span class="sxs-lookup"><span data-stu-id="03604-124">8</span></span>|<span data-ttu-id="03604-125">计算机处于挂起的脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="03604-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="03604-126">关键</span><span class="sxs-lookup"><span data-stu-id="03604-126">critical</span></span>|<span data-ttu-id="03604-127">位</span><span class="sxs-lookup"><span data-stu-id="03604-127">16</span></span>|<span data-ttu-id="03604-128">计算机处于严重故障状态</span><span class="sxs-lookup"><span data-stu-id="03604-128">Computer is in critical failure state</span></span>|




