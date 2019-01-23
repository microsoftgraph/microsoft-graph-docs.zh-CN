---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416347"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="b1184-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1184-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="b1184-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b1184-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1184-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1184-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1184-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1184-107">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="b1184-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="b1184-108">成员</span><span class="sxs-lookup"><span data-stu-id="b1184-108">Members</span></span>
|<span data-ttu-id="b1184-109">成员</span><span class="sxs-lookup"><span data-stu-id="b1184-109">Member</span></span>|<span data-ttu-id="b1184-110">值</span><span class="sxs-lookup"><span data-stu-id="b1184-110">Value</span></span>|<span data-ttu-id="b1184-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1184-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1184-112">clean</span><span class="sxs-lookup"><span data-stu-id="b1184-112">clean</span></span>|<span data-ttu-id="b1184-113">0</span><span class="sxs-lookup"><span data-stu-id="b1184-113">0</span></span>|<span data-ttu-id="b1184-114">计算机的完全而不不需要任何操作</span><span class="sxs-lookup"><span data-stu-id="b1184-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="b1184-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="b1184-115">fullScanPending</span></span>|<span data-ttu-id="b1184-116">1</span><span class="sxs-lookup"><span data-stu-id="b1184-116">1</span></span>|<span data-ttu-id="b1184-117">计算机处于挂起完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="b1184-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="b1184-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="b1184-118">rebootPending</span></span>|<span data-ttu-id="b1184-119">2</span><span class="sxs-lookup"><span data-stu-id="b1184-119">2</span></span>|<span data-ttu-id="b1184-120">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="b1184-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="b1184-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="b1184-121">manualStepsPending</span></span>|<span data-ttu-id="b1184-122">4</span><span class="sxs-lookup"><span data-stu-id="b1184-122">4</span></span>|<span data-ttu-id="b1184-123">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="b1184-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="b1184-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="b1184-124">offlineScanPending</span></span>|<span data-ttu-id="b1184-125">8</span><span class="sxs-lookup"><span data-stu-id="b1184-125">8</span></span>|<span data-ttu-id="b1184-126">计算机处于挂起脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="b1184-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="b1184-127">critical</span><span class="sxs-lookup"><span data-stu-id="b1184-127">critical</span></span>|<span data-ttu-id="b1184-128">16</span><span class="sxs-lookup"><span data-stu-id="b1184-128">16</span></span>|<span data-ttu-id="b1184-129">计算机处于关键失败状态</span><span class="sxs-lookup"><span data-stu-id="b1184-129">Computer is in critical failure state</span></span>|




