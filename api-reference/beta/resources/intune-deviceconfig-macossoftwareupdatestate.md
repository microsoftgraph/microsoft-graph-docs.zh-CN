---
title: macOSSoftwareUpdateState 枚举类型
description: MacOS 软件更新状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 05d2d951d8eacb93d952e20f01af6e42b30eecc1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731076"
---
# <a name="macossoftwareupdatestate-enum-type"></a><span data-ttu-id="e4492-103">macOSSoftwareUpdateState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e4492-103">macOSSoftwareUpdateState enum type</span></span>

<span data-ttu-id="e4492-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4492-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4492-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4492-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4492-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4492-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4492-107">MacOS 软件更新状态</span><span class="sxs-lookup"><span data-stu-id="e4492-107">MacOS Software Update State</span></span>

## <a name="members"></a><span data-ttu-id="e4492-108">成员</span><span class="sxs-lookup"><span data-stu-id="e4492-108">Members</span></span>
|<span data-ttu-id="e4492-109">成员</span><span class="sxs-lookup"><span data-stu-id="e4492-109">Member</span></span>|<span data-ttu-id="e4492-110">值</span><span class="sxs-lookup"><span data-stu-id="e4492-110">Value</span></span>|<span data-ttu-id="e4492-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4492-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4492-112">success</span><span class="sxs-lookup"><span data-stu-id="e4492-112">success</span></span>|<span data-ttu-id="e4492-113">0</span><span class="sxs-lookup"><span data-stu-id="e4492-113">0</span></span>|<span data-ttu-id="e4492-114">成功安装软件更新</span><span class="sxs-lookup"><span data-stu-id="e4492-114">The software update successfully installed</span></span>|
|<span data-ttu-id="e4492-115">下载</span><span class="sxs-lookup"><span data-stu-id="e4492-115">downloading</span></span>|<span data-ttu-id="e4492-116">1000</span><span class="sxs-lookup"><span data-stu-id="e4492-116">1000</span></span>|<span data-ttu-id="e4492-117">正在下载软件更新</span><span class="sxs-lookup"><span data-stu-id="e4492-117">The software update is being downloaded</span></span>|
|<span data-ttu-id="e4492-118">完毕</span><span class="sxs-lookup"><span data-stu-id="e4492-118">downloaded</span></span>|<span data-ttu-id="e4492-119">1001</span><span class="sxs-lookup"><span data-stu-id="e4492-119">1001</span></span>|<span data-ttu-id="e4492-120">已下载软件更新</span><span class="sxs-lookup"><span data-stu-id="e4492-120">The software update has been downloaded</span></span>|
|<span data-ttu-id="e4492-121">安装</span><span class="sxs-lookup"><span data-stu-id="e4492-121">installing</span></span>|<span data-ttu-id="e4492-122">1002</span><span class="sxs-lookup"><span data-stu-id="e4492-122">1002</span></span>|<span data-ttu-id="e4492-123">正在安装软件更新</span><span class="sxs-lookup"><span data-stu-id="e4492-123">The software update is being installed</span></span>|
|<span data-ttu-id="e4492-124">待机</span><span class="sxs-lookup"><span data-stu-id="e4492-124">idle</span></span>|<span data-ttu-id="e4492-125">1003</span><span class="sxs-lookup"><span data-stu-id="e4492-125">1003</span></span>|<span data-ttu-id="e4492-126">对此软件更新不执行任何操作</span><span class="sxs-lookup"><span data-stu-id="e4492-126">No action is being taken on this software update</span></span>|
|<span data-ttu-id="e4492-127">可用</span><span class="sxs-lookup"><span data-stu-id="e4492-127">available</span></span>|<span data-ttu-id="e4492-128">1004</span><span class="sxs-lookup"><span data-stu-id="e4492-128">1004</span></span>|<span data-ttu-id="e4492-129">软件更新在设备上可用</span><span class="sxs-lookup"><span data-stu-id="e4492-129">The software update is available on the device</span></span>|
|<span data-ttu-id="e4492-130">scheduled</span><span class="sxs-lookup"><span data-stu-id="e4492-130">scheduled</span></span>|<span data-ttu-id="e4492-131">1005</span><span class="sxs-lookup"><span data-stu-id="e4492-131">1005</span></span>|<span data-ttu-id="e4492-132">已在设备上安排软件更新</span><span class="sxs-lookup"><span data-stu-id="e4492-132">The software update has been scheduled on the device</span></span>|
|<span data-ttu-id="e4492-133">downloadFailed</span><span class="sxs-lookup"><span data-stu-id="e4492-133">downloadFailed</span></span>|<span data-ttu-id="e4492-134">2000</span><span class="sxs-lookup"><span data-stu-id="e4492-134">2000</span></span>|<span data-ttu-id="e4492-135">软件更新下载失败</span><span class="sxs-lookup"><span data-stu-id="e4492-135">The software update download has failed</span></span>|
|<span data-ttu-id="e4492-136">downloadInsufficientSpace</span><span class="sxs-lookup"><span data-stu-id="e4492-136">downloadInsufficientSpace</span></span>|<span data-ttu-id="e4492-137">2001</span><span class="sxs-lookup"><span data-stu-id="e4492-137">2001</span></span>|<span data-ttu-id="e4492-138">空间不足，无法下载更新</span><span class="sxs-lookup"><span data-stu-id="e4492-138">There is not enough space to download the update</span></span>|
|<span data-ttu-id="e4492-139">downloadInsufficientPower</span><span class="sxs-lookup"><span data-stu-id="e4492-139">downloadInsufficientPower</span></span>|<span data-ttu-id="e4492-140">2002</span><span class="sxs-lookup"><span data-stu-id="e4492-140">2002</span></span>|<span data-ttu-id="e4492-141">没有足够的功率来下载更新</span><span class="sxs-lookup"><span data-stu-id="e4492-141">There is not enough power to download the update</span></span>|
|<span data-ttu-id="e4492-142">downloadInsufficientNetwork</span><span class="sxs-lookup"><span data-stu-id="e4492-142">downloadInsufficientNetwork</span></span>|<span data-ttu-id="e4492-143">2003</span><span class="sxs-lookup"><span data-stu-id="e4492-143">2003</span></span>|<span data-ttu-id="e4492-144">网络容量不足，无法下载更新</span><span class="sxs-lookup"><span data-stu-id="e4492-144">There is insufficient network capacity to download the update</span></span>|
|<span data-ttu-id="e4492-145">installInsufficientSpace</span><span class="sxs-lookup"><span data-stu-id="e4492-145">installInsufficientSpace</span></span>|<span data-ttu-id="e4492-146">2004</span><span class="sxs-lookup"><span data-stu-id="e4492-146">2004</span></span>|<span data-ttu-id="e4492-147">空间不足，无法安装更新</span><span class="sxs-lookup"><span data-stu-id="e4492-147">There is not enough space to install the update</span></span>|
|<span data-ttu-id="e4492-148">installInsufficientPower</span><span class="sxs-lookup"><span data-stu-id="e4492-148">installInsufficientPower</span></span>|<span data-ttu-id="e4492-149">2005</span><span class="sxs-lookup"><span data-stu-id="e4492-149">2005</span></span>|<span data-ttu-id="e4492-150">没有足够的电源来安装更新</span><span class="sxs-lookup"><span data-stu-id="e4492-150">There is not enough power to install the update</span></span>|
|<span data-ttu-id="e4492-151">installFailed</span><span class="sxs-lookup"><span data-stu-id="e4492-151">installFailed</span></span>|<span data-ttu-id="e4492-152">2006</span><span class="sxs-lookup"><span data-stu-id="e4492-152">2006</span></span>|<span data-ttu-id="e4492-153">安装因未指定原因而失败</span><span class="sxs-lookup"><span data-stu-id="e4492-153">Installation has failed for an unspecified reason</span></span>|
|<span data-ttu-id="e4492-154">commandFailed</span><span class="sxs-lookup"><span data-stu-id="e4492-154">commandFailed</span></span>|<span data-ttu-id="e4492-155">2007</span><span class="sxs-lookup"><span data-stu-id="e4492-155">2007</span></span>|<span data-ttu-id="e4492-156">由于未指定的原因，计划更新命令失败</span><span class="sxs-lookup"><span data-stu-id="e4492-156">The schedule update command has failed for an unspecified reason</span></span>|





