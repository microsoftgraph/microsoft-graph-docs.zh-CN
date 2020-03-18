---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69d20e06ba23390ff912251bb99980c4a945704c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783709"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="18d62-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="18d62-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="18d62-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18d62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18d62-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18d62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d62-106">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="18d62-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="18d62-107">成员</span><span class="sxs-lookup"><span data-stu-id="18d62-107">Members</span></span>
|<span data-ttu-id="18d62-108">成员</span><span class="sxs-lookup"><span data-stu-id="18d62-108">Member</span></span>|<span data-ttu-id="18d62-109">值</span><span class="sxs-lookup"><span data-stu-id="18d62-109">Value</span></span>|<span data-ttu-id="18d62-110">说明</span><span class="sxs-lookup"><span data-stu-id="18d62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d62-111">清理</span><span class="sxs-lookup"><span data-stu-id="18d62-111">clean</span></span>|<span data-ttu-id="18d62-112">0</span><span class="sxs-lookup"><span data-stu-id="18d62-112">0</span></span>|<span data-ttu-id="18d62-113">计算机干净，无需任何操作</span><span class="sxs-lookup"><span data-stu-id="18d62-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="18d62-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="18d62-114">fullScanPending</span></span>|<span data-ttu-id="18d62-115">1</span><span class="sxs-lookup"><span data-stu-id="18d62-115">1</span></span>|<span data-ttu-id="18d62-116">计算机处于挂起的完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="18d62-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="18d62-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="18d62-117">rebootPending</span></span>|<span data-ttu-id="18d62-118">双面</span><span class="sxs-lookup"><span data-stu-id="18d62-118">2</span></span>|<span data-ttu-id="18d62-119">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="18d62-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="18d62-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="18d62-120">manualStepsPending</span></span>|<span data-ttu-id="18d62-121">4 </span><span class="sxs-lookup"><span data-stu-id="18d62-121">4</span></span>|<span data-ttu-id="18d62-122">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="18d62-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="18d62-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="18d62-123">offlineScanPending</span></span>|<span data-ttu-id="18d62-124">8 </span><span class="sxs-lookup"><span data-stu-id="18d62-124">8</span></span>|<span data-ttu-id="18d62-125">计算机处于挂起的脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="18d62-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="18d62-126">关键</span><span class="sxs-lookup"><span data-stu-id="18d62-126">critical</span></span>|<span data-ttu-id="18d62-127">16 </span><span class="sxs-lookup"><span data-stu-id="18d62-127">16</span></span>|<span data-ttu-id="18d62-128">计算机处于严重故障状态</span><span class="sxs-lookup"><span data-stu-id="18d62-128">Computer is in critical failure state</span></span>|



