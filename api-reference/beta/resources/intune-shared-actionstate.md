---
title: actionState 枚举类型
description: 设备上操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d55ff0419c6178668bbee921c149c8bc797ebff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143398"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="82f97-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="82f97-103">actionState enum type</span></span>

> <span data-ttu-id="82f97-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82f97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82f97-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82f97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82f97-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="82f97-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="82f97-107">成员</span><span class="sxs-lookup"><span data-stu-id="82f97-107">Members</span></span>
|<span data-ttu-id="82f97-108">成员</span><span class="sxs-lookup"><span data-stu-id="82f97-108">Member</span></span>|<span data-ttu-id="82f97-109">值</span><span class="sxs-lookup"><span data-stu-id="82f97-109">Value</span></span>|<span data-ttu-id="82f97-110">说明</span><span class="sxs-lookup"><span data-stu-id="82f97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82f97-111">无</span><span class="sxs-lookup"><span data-stu-id="82f97-111">none</span></span>|<span data-ttu-id="82f97-112">0</span><span class="sxs-lookup"><span data-stu-id="82f97-112">0</span></span>|<span data-ttu-id="82f97-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="82f97-113">Not a valid action state</span></span>|
|<span data-ttu-id="82f97-114">决</span><span class="sxs-lookup"><span data-stu-id="82f97-114">pending</span></span>|<span data-ttu-id="82f97-115">1</span><span class="sxs-lookup"><span data-stu-id="82f97-115">1</span></span>|<span data-ttu-id="82f97-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="82f97-116">Action is pending</span></span>|
|<span data-ttu-id="82f97-117">取消</span><span class="sxs-lookup"><span data-stu-id="82f97-117">canceled</span></span>|<span data-ttu-id="82f97-118">双面</span><span class="sxs-lookup"><span data-stu-id="82f97-118">2</span></span>|<span data-ttu-id="82f97-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="82f97-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="82f97-120">工作</span><span class="sxs-lookup"><span data-stu-id="82f97-120">active</span></span>|<span data-ttu-id="82f97-121">第三章</span><span class="sxs-lookup"><span data-stu-id="82f97-121">3</span></span>|<span data-ttu-id="82f97-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="82f97-122">Action is active.</span></span>|
|<span data-ttu-id="82f97-123">done</span><span class="sxs-lookup"><span data-stu-id="82f97-123">done</span></span>|<span data-ttu-id="82f97-124">4</span><span class="sxs-lookup"><span data-stu-id="82f97-124">4</span></span>|<span data-ttu-id="82f97-125">操作已完成, 无错误。</span><span class="sxs-lookup"><span data-stu-id="82f97-125">Action completed without errors.</span></span>|
|<span data-ttu-id="82f97-126">failed</span><span class="sxs-lookup"><span data-stu-id="82f97-126">failed</span></span>|<span data-ttu-id="82f97-127">5</span><span class="sxs-lookup"><span data-stu-id="82f97-127">5</span></span>|<span data-ttu-id="82f97-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="82f97-128">Action failed</span></span>|
|<span data-ttu-id="82f97-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="82f97-129">notSupported</span></span>|<span data-ttu-id="82f97-130">型</span><span class="sxs-lookup"><span data-stu-id="82f97-130">6</span></span>|<span data-ttu-id="82f97-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="82f97-131">Action is not supported.</span></span>|




