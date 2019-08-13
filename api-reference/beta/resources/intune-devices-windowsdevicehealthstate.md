---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b37f441a1ded71d3f299d6d38b58543aac130ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366448"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="f0b6e-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f0b6e-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="f0b6e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0b6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0b6e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0b6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b6e-106">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="f0b6e-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="f0b6e-107">成员</span><span class="sxs-lookup"><span data-stu-id="f0b6e-107">Members</span></span>
|<span data-ttu-id="f0b6e-108">成员</span><span class="sxs-lookup"><span data-stu-id="f0b6e-108">Member</span></span>|<span data-ttu-id="f0b6e-109">值</span><span class="sxs-lookup"><span data-stu-id="f0b6e-109">Value</span></span>|<span data-ttu-id="f0b6e-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0b6e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b6e-111">清理</span><span class="sxs-lookup"><span data-stu-id="f0b6e-111">clean</span></span>|<span data-ttu-id="f0b6e-112">0</span><span class="sxs-lookup"><span data-stu-id="f0b6e-112">0</span></span>|<span data-ttu-id="f0b6e-113">计算机干净, 无需任何操作</span><span class="sxs-lookup"><span data-stu-id="f0b6e-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="f0b6e-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="f0b6e-114">fullScanPending</span></span>|<span data-ttu-id="f0b6e-115">1</span><span class="sxs-lookup"><span data-stu-id="f0b6e-115">1</span></span>|<span data-ttu-id="f0b6e-116">计算机处于挂起的完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="f0b6e-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="f0b6e-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="f0b6e-117">rebootPending</span></span>|<span data-ttu-id="f0b6e-118">双面</span><span class="sxs-lookup"><span data-stu-id="f0b6e-118">2</span></span>|<span data-ttu-id="f0b6e-119">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="f0b6e-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="f0b6e-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="f0b6e-120">manualStepsPending</span></span>|<span data-ttu-id="f0b6e-121">4</span><span class="sxs-lookup"><span data-stu-id="f0b6e-121">4</span></span>|<span data-ttu-id="f0b6e-122">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="f0b6e-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="f0b6e-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="f0b6e-123">offlineScanPending</span></span>|<span data-ttu-id="f0b6e-124">utf-8</span><span class="sxs-lookup"><span data-stu-id="f0b6e-124">8</span></span>|<span data-ttu-id="f0b6e-125">计算机处于挂起的脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="f0b6e-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="f0b6e-126">关键</span><span class="sxs-lookup"><span data-stu-id="f0b6e-126">critical</span></span>|<span data-ttu-id="f0b6e-127">位</span><span class="sxs-lookup"><span data-stu-id="f0b6e-127">16</span></span>|<span data-ttu-id="f0b6e-128">计算机处于严重故障状态</span><span class="sxs-lookup"><span data-stu-id="f0b6e-128">Computer is in critical failure state</span></span>|



