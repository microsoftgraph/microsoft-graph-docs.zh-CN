---
title: userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型
description: 操作系统重新启动类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9768f77cacb98436b947a516a4ce769798679f1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226361"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="e4a6b-103">userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e4a6b-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="e4a6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4a6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4a6b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4a6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4a6b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4a6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4a6b-107">操作系统重新启动类别</span><span class="sxs-lookup"><span data-stu-id="e4a6b-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="e4a6b-108">成员</span><span class="sxs-lookup"><span data-stu-id="e4a6b-108">Members</span></span>
|<span data-ttu-id="e4a6b-109">成员</span><span class="sxs-lookup"><span data-stu-id="e4a6b-109">Member</span></span>|<span data-ttu-id="e4a6b-110">值</span><span class="sxs-lookup"><span data-stu-id="e4a6b-110">Value</span></span>|<span data-ttu-id="e4a6b-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4a6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a6b-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e4a6b-112">unknown</span></span>|<span data-ttu-id="e4a6b-113">0</span><span class="sxs-lookup"><span data-stu-id="e4a6b-113">0</span></span>|<span data-ttu-id="e4a6b-114">未知</span><span class="sxs-lookup"><span data-stu-id="e4a6b-114">Unknown</span></span>|
|<span data-ttu-id="e4a6b-115">restartWithUpdate</span><span class="sxs-lookup"><span data-stu-id="e4a6b-115">restartWithUpdate</span></span>|<span data-ttu-id="e4a6b-116">1</span><span class="sxs-lookup"><span data-stu-id="e4a6b-116">1</span></span>|<span data-ttu-id="e4a6b-117">重新启动并更新</span><span class="sxs-lookup"><span data-stu-id="e4a6b-117">Restart with update</span></span>|
|<span data-ttu-id="e4a6b-118">restartWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="e4a6b-118">restartWithoutUpdate</span></span>|<span data-ttu-id="e4a6b-119">双面</span><span class="sxs-lookup"><span data-stu-id="e4a6b-119">2</span></span>|<span data-ttu-id="e4a6b-120">重新启动而不更新</span><span class="sxs-lookup"><span data-stu-id="e4a6b-120">Restart without update</span></span>|
|<span data-ttu-id="e4a6b-121">Options.bluescreen</span><span class="sxs-lookup"><span data-stu-id="e4a6b-121">blueScreen</span></span>|<span data-ttu-id="e4a6b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e4a6b-122">3</span></span>|<span data-ttu-id="e4a6b-123">蓝屏重启</span><span class="sxs-lookup"><span data-stu-id="e4a6b-123">Blue screen restart</span></span>|
|<span data-ttu-id="e4a6b-124">shutdownWithUpdate</span><span class="sxs-lookup"><span data-stu-id="e4a6b-124">shutdownWithUpdate</span></span>|<span data-ttu-id="e4a6b-125">4 </span><span class="sxs-lookup"><span data-stu-id="e4a6b-125">4</span></span>|<span data-ttu-id="e4a6b-126">使用更新进行关机</span><span class="sxs-lookup"><span data-stu-id="e4a6b-126">Shutdown with update</span></span>|
|<span data-ttu-id="e4a6b-127">shutdownWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="e4a6b-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="e4a6b-128">5 </span><span class="sxs-lookup"><span data-stu-id="e4a6b-128">5</span></span>|<span data-ttu-id="e4a6b-129">关闭而不更新</span><span class="sxs-lookup"><span data-stu-id="e4a6b-129">Shutdown without update</span></span>|
|<span data-ttu-id="e4a6b-130">longPowerButtonPress</span><span class="sxs-lookup"><span data-stu-id="e4a6b-130">longPowerButtonPress</span></span>|<span data-ttu-id="e4a6b-131">6 </span><span class="sxs-lookup"><span data-stu-id="e4a6b-131">6</span></span>|<span data-ttu-id="e4a6b-132">长电源按钮按下</span><span class="sxs-lookup"><span data-stu-id="e4a6b-132">Long power button press</span></span>|
|<span data-ttu-id="e4a6b-133">bootError</span><span class="sxs-lookup"><span data-stu-id="e4a6b-133">bootError</span></span>|<span data-ttu-id="e4a6b-134">7 </span><span class="sxs-lookup"><span data-stu-id="e4a6b-134">7</span></span>|<span data-ttu-id="e4a6b-135">启动错误</span><span class="sxs-lookup"><span data-stu-id="e4a6b-135">Boot error</span></span>|




