---
title: userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型
description: 操作系统重新启动类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 69cac1316054a7822cb169eb4070a8787c101032
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697635"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="57fca-103">userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型</span><span class="sxs-lookup"><span data-stu-id="57fca-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="57fca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57fca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57fca-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57fca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57fca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57fca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57fca-107">操作系统重新启动类别</span><span class="sxs-lookup"><span data-stu-id="57fca-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="57fca-108">成员</span><span class="sxs-lookup"><span data-stu-id="57fca-108">Members</span></span>
|<span data-ttu-id="57fca-109">成员</span><span class="sxs-lookup"><span data-stu-id="57fca-109">Member</span></span>|<span data-ttu-id="57fca-110">值</span><span class="sxs-lookup"><span data-stu-id="57fca-110">Value</span></span>|<span data-ttu-id="57fca-111">说明</span><span class="sxs-lookup"><span data-stu-id="57fca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57fca-112">unknown</span><span class="sxs-lookup"><span data-stu-id="57fca-112">unknown</span></span>|<span data-ttu-id="57fca-113">0</span><span class="sxs-lookup"><span data-stu-id="57fca-113">0</span></span>|<span data-ttu-id="57fca-114">未知</span><span class="sxs-lookup"><span data-stu-id="57fca-114">Unknown</span></span>|
|<span data-ttu-id="57fca-115">restartWithUpdate</span><span class="sxs-lookup"><span data-stu-id="57fca-115">restartWithUpdate</span></span>|<span data-ttu-id="57fca-116">1</span><span class="sxs-lookup"><span data-stu-id="57fca-116">1</span></span>|<span data-ttu-id="57fca-117">重新启动并更新</span><span class="sxs-lookup"><span data-stu-id="57fca-117">Restart with update</span></span>|
|<span data-ttu-id="57fca-118">restartWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="57fca-118">restartWithoutUpdate</span></span>|<span data-ttu-id="57fca-119">双面</span><span class="sxs-lookup"><span data-stu-id="57fca-119">2</span></span>|<span data-ttu-id="57fca-120">重新启动而不更新</span><span class="sxs-lookup"><span data-stu-id="57fca-120">Restart without update</span></span>|
|<span data-ttu-id="57fca-121">Options.bluescreen</span><span class="sxs-lookup"><span data-stu-id="57fca-121">blueScreen</span></span>|<span data-ttu-id="57fca-122">第三章</span><span class="sxs-lookup"><span data-stu-id="57fca-122">3</span></span>|<span data-ttu-id="57fca-123">蓝屏重启</span><span class="sxs-lookup"><span data-stu-id="57fca-123">Blue screen restart</span></span>|
|<span data-ttu-id="57fca-124">shutdownWithUpdate</span><span class="sxs-lookup"><span data-stu-id="57fca-124">shutdownWithUpdate</span></span>|<span data-ttu-id="57fca-125">4 </span><span class="sxs-lookup"><span data-stu-id="57fca-125">4</span></span>|<span data-ttu-id="57fca-126">使用更新进行关机</span><span class="sxs-lookup"><span data-stu-id="57fca-126">Shutdown with update</span></span>|
|<span data-ttu-id="57fca-127">shutdownWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="57fca-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="57fca-128">5 </span><span class="sxs-lookup"><span data-stu-id="57fca-128">5</span></span>|<span data-ttu-id="57fca-129">关闭而不更新</span><span class="sxs-lookup"><span data-stu-id="57fca-129">Shutdown without update</span></span>|
|<span data-ttu-id="57fca-130">longPowerButtonPress</span><span class="sxs-lookup"><span data-stu-id="57fca-130">longPowerButtonPress</span></span>|<span data-ttu-id="57fca-131">6 </span><span class="sxs-lookup"><span data-stu-id="57fca-131">6</span></span>|<span data-ttu-id="57fca-132">长电源按钮按下</span><span class="sxs-lookup"><span data-stu-id="57fca-132">Long power button press</span></span>|
|<span data-ttu-id="57fca-133">bootError</span><span class="sxs-lookup"><span data-stu-id="57fca-133">bootError</span></span>|<span data-ttu-id="57fca-134">7 </span><span class="sxs-lookup"><span data-stu-id="57fca-134">7</span></span>|<span data-ttu-id="57fca-135">启动错误</span><span class="sxs-lookup"><span data-stu-id="57fca-135">Boot error</span></span>|





