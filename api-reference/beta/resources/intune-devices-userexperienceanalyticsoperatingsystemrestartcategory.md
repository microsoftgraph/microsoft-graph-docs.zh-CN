---
title: userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型
description: 操作系统重启类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d298545fae20b123440b86a475b713686ae65ea4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156810"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="84ba9-103">userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型</span><span class="sxs-lookup"><span data-stu-id="84ba9-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="84ba9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ba9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ba9-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84ba9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ba9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84ba9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ba9-107">操作系统重启类别</span><span class="sxs-lookup"><span data-stu-id="84ba9-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="84ba9-108">成员</span><span class="sxs-lookup"><span data-stu-id="84ba9-108">Members</span></span>
|<span data-ttu-id="84ba9-109">成员</span><span class="sxs-lookup"><span data-stu-id="84ba9-109">Member</span></span>|<span data-ttu-id="84ba9-110">值</span><span class="sxs-lookup"><span data-stu-id="84ba9-110">Value</span></span>|<span data-ttu-id="84ba9-111">说明</span><span class="sxs-lookup"><span data-stu-id="84ba9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ba9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="84ba9-112">unknown</span></span>|<span data-ttu-id="84ba9-113">0</span><span class="sxs-lookup"><span data-stu-id="84ba9-113">0</span></span>|<span data-ttu-id="84ba9-114">未知</span><span class="sxs-lookup"><span data-stu-id="84ba9-114">Unknown</span></span>|
|<span data-ttu-id="84ba9-115">restartWithUpdate</span><span class="sxs-lookup"><span data-stu-id="84ba9-115">restartWithUpdate</span></span>|<span data-ttu-id="84ba9-116">1 </span><span class="sxs-lookup"><span data-stu-id="84ba9-116">1</span></span>|<span data-ttu-id="84ba9-117">使用更新重启</span><span class="sxs-lookup"><span data-stu-id="84ba9-117">Restart with update</span></span>|
|<span data-ttu-id="84ba9-118">restartWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="84ba9-118">restartWithoutUpdate</span></span>|<span data-ttu-id="84ba9-119">2 </span><span class="sxs-lookup"><span data-stu-id="84ba9-119">2</span></span>|<span data-ttu-id="84ba9-120">在不更新的情况下重启</span><span class="sxs-lookup"><span data-stu-id="84ba9-120">Restart without update</span></span>|
|<span data-ttu-id="84ba9-121">blueScreen</span><span class="sxs-lookup"><span data-stu-id="84ba9-121">blueScreen</span></span>|<span data-ttu-id="84ba9-122">3 </span><span class="sxs-lookup"><span data-stu-id="84ba9-122">3</span></span>|<span data-ttu-id="84ba9-123">蓝屏重启</span><span class="sxs-lookup"><span data-stu-id="84ba9-123">Blue screen restart</span></span>|
|<span data-ttu-id="84ba9-124">shutdownWithUpdate</span><span class="sxs-lookup"><span data-stu-id="84ba9-124">shutdownWithUpdate</span></span>|<span data-ttu-id="84ba9-125">4 </span><span class="sxs-lookup"><span data-stu-id="84ba9-125">4</span></span>|<span data-ttu-id="84ba9-126">通过更新关闭</span><span class="sxs-lookup"><span data-stu-id="84ba9-126">Shutdown with update</span></span>|
|<span data-ttu-id="84ba9-127">shutdownWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="84ba9-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="84ba9-128">5 </span><span class="sxs-lookup"><span data-stu-id="84ba9-128">5</span></span>|<span data-ttu-id="84ba9-129">关闭而不更新</span><span class="sxs-lookup"><span data-stu-id="84ba9-129">Shutdown without update</span></span>|
|<span data-ttu-id="84ba9-130">longPowerButtonPress</span><span class="sxs-lookup"><span data-stu-id="84ba9-130">longPowerButtonPress</span></span>|<span data-ttu-id="84ba9-131">6 </span><span class="sxs-lookup"><span data-stu-id="84ba9-131">6</span></span>|<span data-ttu-id="84ba9-132">长按电源按钮</span><span class="sxs-lookup"><span data-stu-id="84ba9-132">Long power button press</span></span>|
|<span data-ttu-id="84ba9-133">bootError</span><span class="sxs-lookup"><span data-stu-id="84ba9-133">bootError</span></span>|<span data-ttu-id="84ba9-134">7 </span><span class="sxs-lookup"><span data-stu-id="84ba9-134">7</span></span>|<span data-ttu-id="84ba9-135">启动错误</span><span class="sxs-lookup"><span data-stu-id="84ba9-135">Boot error</span></span>|
|<span data-ttu-id="84ba9-136">update</span><span class="sxs-lookup"><span data-stu-id="84ba9-136">update</span></span>|<span data-ttu-id="84ba9-137">8 </span><span class="sxs-lookup"><span data-stu-id="84ba9-137">8</span></span>|<span data-ttu-id="84ba9-138">更新</span><span class="sxs-lookup"><span data-stu-id="84ba9-138">Update</span></span>|




