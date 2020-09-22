---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c24f0b022d60ef6a9b50d881fdaa05b88bd518c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080654"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="4f325-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4f325-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="4f325-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f325-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f325-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f325-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f325-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f325-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f325-107">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="4f325-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="4f325-108">成员</span><span class="sxs-lookup"><span data-stu-id="4f325-108">Members</span></span>
|<span data-ttu-id="4f325-109">成员</span><span class="sxs-lookup"><span data-stu-id="4f325-109">Member</span></span>|<span data-ttu-id="4f325-110">值</span><span class="sxs-lookup"><span data-stu-id="4f325-110">Value</span></span>|<span data-ttu-id="4f325-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f325-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f325-112">清理</span><span class="sxs-lookup"><span data-stu-id="4f325-112">clean</span></span>|<span data-ttu-id="4f325-113">0</span><span class="sxs-lookup"><span data-stu-id="4f325-113">0</span></span>|<span data-ttu-id="4f325-114">计算机干净，无需任何操作</span><span class="sxs-lookup"><span data-stu-id="4f325-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="4f325-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="4f325-115">fullScanPending</span></span>|<span data-ttu-id="4f325-116">1 </span><span class="sxs-lookup"><span data-stu-id="4f325-116">1</span></span>|<span data-ttu-id="4f325-117">计算机处于挂起的完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="4f325-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="4f325-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="4f325-118">rebootPending</span></span>|<span data-ttu-id="4f325-119">2 </span><span class="sxs-lookup"><span data-stu-id="4f325-119">2</span></span>|<span data-ttu-id="4f325-120">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="4f325-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="4f325-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="4f325-121">manualStepsPending</span></span>|<span data-ttu-id="4f325-122">4 </span><span class="sxs-lookup"><span data-stu-id="4f325-122">4</span></span>|<span data-ttu-id="4f325-123">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="4f325-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="4f325-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="4f325-124">offlineScanPending</span></span>|<span data-ttu-id="4f325-125">8 </span><span class="sxs-lookup"><span data-stu-id="4f325-125">8</span></span>|<span data-ttu-id="4f325-126">计算机处于挂起的脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="4f325-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="4f325-127">关键</span><span class="sxs-lookup"><span data-stu-id="4f325-127">critical</span></span>|<span data-ttu-id="4f325-128">16 </span><span class="sxs-lookup"><span data-stu-id="4f325-128">16</span></span>|<span data-ttu-id="4f325-129">计算机处于严重故障状态</span><span class="sxs-lookup"><span data-stu-id="4f325-129">Computer is in critical failure state</span></span>|






