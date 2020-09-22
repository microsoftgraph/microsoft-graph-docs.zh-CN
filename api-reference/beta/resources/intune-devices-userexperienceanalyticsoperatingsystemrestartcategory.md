---
title: userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型
description: 操作系统重新启动类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d78328cc9f44dbffca0085890a8c69184c2eac3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080801"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="ab7dd-103">userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab7dd-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="ab7dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab7dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab7dd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab7dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab7dd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab7dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab7dd-107">操作系统重新启动类别</span><span class="sxs-lookup"><span data-stu-id="ab7dd-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="ab7dd-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab7dd-108">Members</span></span>
|<span data-ttu-id="ab7dd-109">成员</span><span class="sxs-lookup"><span data-stu-id="ab7dd-109">Member</span></span>|<span data-ttu-id="ab7dd-110">值</span><span class="sxs-lookup"><span data-stu-id="ab7dd-110">Value</span></span>|<span data-ttu-id="ab7dd-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab7dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab7dd-112">unknown</span><span class="sxs-lookup"><span data-stu-id="ab7dd-112">unknown</span></span>|<span data-ttu-id="ab7dd-113">0</span><span class="sxs-lookup"><span data-stu-id="ab7dd-113">0</span></span>|<span data-ttu-id="ab7dd-114">未知</span><span class="sxs-lookup"><span data-stu-id="ab7dd-114">Unknown</span></span>|
|<span data-ttu-id="ab7dd-115">restartWithUpdate</span><span class="sxs-lookup"><span data-stu-id="ab7dd-115">restartWithUpdate</span></span>|<span data-ttu-id="ab7dd-116">1 </span><span class="sxs-lookup"><span data-stu-id="ab7dd-116">1</span></span>|<span data-ttu-id="ab7dd-117">重新启动并更新</span><span class="sxs-lookup"><span data-stu-id="ab7dd-117">Restart with update</span></span>|
|<span data-ttu-id="ab7dd-118">restartWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="ab7dd-118">restartWithoutUpdate</span></span>|<span data-ttu-id="ab7dd-119">2 </span><span class="sxs-lookup"><span data-stu-id="ab7dd-119">2</span></span>|<span data-ttu-id="ab7dd-120">重新启动而不更新</span><span class="sxs-lookup"><span data-stu-id="ab7dd-120">Restart without update</span></span>|
|<span data-ttu-id="ab7dd-121">Options.bluescreen</span><span class="sxs-lookup"><span data-stu-id="ab7dd-121">blueScreen</span></span>|<span data-ttu-id="ab7dd-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ab7dd-122">3</span></span>|<span data-ttu-id="ab7dd-123">蓝屏重启</span><span class="sxs-lookup"><span data-stu-id="ab7dd-123">Blue screen restart</span></span>|
|<span data-ttu-id="ab7dd-124">shutdownWithUpdate</span><span class="sxs-lookup"><span data-stu-id="ab7dd-124">shutdownWithUpdate</span></span>|<span data-ttu-id="ab7dd-125">4 </span><span class="sxs-lookup"><span data-stu-id="ab7dd-125">4</span></span>|<span data-ttu-id="ab7dd-126">使用更新进行关机</span><span class="sxs-lookup"><span data-stu-id="ab7dd-126">Shutdown with update</span></span>|
|<span data-ttu-id="ab7dd-127">shutdownWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="ab7dd-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="ab7dd-128">5 </span><span class="sxs-lookup"><span data-stu-id="ab7dd-128">5</span></span>|<span data-ttu-id="ab7dd-129">关闭而不更新</span><span class="sxs-lookup"><span data-stu-id="ab7dd-129">Shutdown without update</span></span>|
|<span data-ttu-id="ab7dd-130">longPowerButtonPress</span><span class="sxs-lookup"><span data-stu-id="ab7dd-130">longPowerButtonPress</span></span>|<span data-ttu-id="ab7dd-131">6 </span><span class="sxs-lookup"><span data-stu-id="ab7dd-131">6</span></span>|<span data-ttu-id="ab7dd-132">长电源按钮按下</span><span class="sxs-lookup"><span data-stu-id="ab7dd-132">Long power button press</span></span>|
|<span data-ttu-id="ab7dd-133">bootError</span><span class="sxs-lookup"><span data-stu-id="ab7dd-133">bootError</span></span>|<span data-ttu-id="ab7dd-134">7 </span><span class="sxs-lookup"><span data-stu-id="ab7dd-134">7</span></span>|<span data-ttu-id="ab7dd-135">启动错误</span><span class="sxs-lookup"><span data-stu-id="ab7dd-135">Boot error</span></span>|






