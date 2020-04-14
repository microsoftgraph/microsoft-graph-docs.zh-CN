---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ce06c1b6c52266bb7d052a4524c6f4439973bde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401748"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="35d86-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="35d86-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="35d86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35d86-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35d86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d86-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35d86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d86-107">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="35d86-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="35d86-108">成员</span><span class="sxs-lookup"><span data-stu-id="35d86-108">Members</span></span>
|<span data-ttu-id="35d86-109">成员</span><span class="sxs-lookup"><span data-stu-id="35d86-109">Member</span></span>|<span data-ttu-id="35d86-110">值</span><span class="sxs-lookup"><span data-stu-id="35d86-110">Value</span></span>|<span data-ttu-id="35d86-111">说明</span><span class="sxs-lookup"><span data-stu-id="35d86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d86-112">清理</span><span class="sxs-lookup"><span data-stu-id="35d86-112">clean</span></span>|<span data-ttu-id="35d86-113">0</span><span class="sxs-lookup"><span data-stu-id="35d86-113">0</span></span>|<span data-ttu-id="35d86-114">计算机干净，无需任何操作</span><span class="sxs-lookup"><span data-stu-id="35d86-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="35d86-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="35d86-115">fullScanPending</span></span>|<span data-ttu-id="35d86-116">1</span><span class="sxs-lookup"><span data-stu-id="35d86-116">1</span></span>|<span data-ttu-id="35d86-117">计算机处于挂起的完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="35d86-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="35d86-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="35d86-118">rebootPending</span></span>|<span data-ttu-id="35d86-119">双面</span><span class="sxs-lookup"><span data-stu-id="35d86-119">2</span></span>|<span data-ttu-id="35d86-120">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="35d86-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="35d86-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="35d86-121">manualStepsPending</span></span>|<span data-ttu-id="35d86-122">4 </span><span class="sxs-lookup"><span data-stu-id="35d86-122">4</span></span>|<span data-ttu-id="35d86-123">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="35d86-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="35d86-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="35d86-124">offlineScanPending</span></span>|<span data-ttu-id="35d86-125">8 </span><span class="sxs-lookup"><span data-stu-id="35d86-125">8</span></span>|<span data-ttu-id="35d86-126">计算机处于挂起的脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="35d86-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="35d86-127">关键</span><span class="sxs-lookup"><span data-stu-id="35d86-127">critical</span></span>|<span data-ttu-id="35d86-128">16 </span><span class="sxs-lookup"><span data-stu-id="35d86-128">16</span></span>|<span data-ttu-id="35d86-129">计算机处于严重故障状态</span><span class="sxs-lookup"><span data-stu-id="35d86-129">Computer is in critical failure state</span></span>|



