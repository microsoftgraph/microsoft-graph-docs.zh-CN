---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f75622021616ac0d65dd305c75d73af738f3446c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733166"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="2406e-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2406e-103">actionState enum type</span></span>

<span data-ttu-id="2406e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2406e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2406e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2406e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2406e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2406e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2406e-107">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="2406e-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="2406e-108">成员</span><span class="sxs-lookup"><span data-stu-id="2406e-108">Members</span></span>
|<span data-ttu-id="2406e-109">成员</span><span class="sxs-lookup"><span data-stu-id="2406e-109">Member</span></span>|<span data-ttu-id="2406e-110">值</span><span class="sxs-lookup"><span data-stu-id="2406e-110">Value</span></span>|<span data-ttu-id="2406e-111">说明</span><span class="sxs-lookup"><span data-stu-id="2406e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2406e-112">无</span><span class="sxs-lookup"><span data-stu-id="2406e-112">none</span></span>|<span data-ttu-id="2406e-113">0</span><span class="sxs-lookup"><span data-stu-id="2406e-113">0</span></span>|<span data-ttu-id="2406e-114">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="2406e-114">Not a valid action state</span></span>|
|<span data-ttu-id="2406e-115">决</span><span class="sxs-lookup"><span data-stu-id="2406e-115">pending</span></span>|<span data-ttu-id="2406e-116">1</span><span class="sxs-lookup"><span data-stu-id="2406e-116">1</span></span>|<span data-ttu-id="2406e-117">操作挂起</span><span class="sxs-lookup"><span data-stu-id="2406e-117">Action is pending</span></span>|
|<span data-ttu-id="2406e-118">取消</span><span class="sxs-lookup"><span data-stu-id="2406e-118">canceled</span></span>|<span data-ttu-id="2406e-119">双面</span><span class="sxs-lookup"><span data-stu-id="2406e-119">2</span></span>|<span data-ttu-id="2406e-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="2406e-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="2406e-121">工作</span><span class="sxs-lookup"><span data-stu-id="2406e-121">active</span></span>|<span data-ttu-id="2406e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="2406e-122">3</span></span>|<span data-ttu-id="2406e-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="2406e-123">Action is active.</span></span>|
|<span data-ttu-id="2406e-124">done</span><span class="sxs-lookup"><span data-stu-id="2406e-124">done</span></span>|<span data-ttu-id="2406e-125">4 </span><span class="sxs-lookup"><span data-stu-id="2406e-125">4</span></span>|<span data-ttu-id="2406e-126">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="2406e-126">Action completed without errors.</span></span>|
|<span data-ttu-id="2406e-127">未能</span><span class="sxs-lookup"><span data-stu-id="2406e-127">failed</span></span>|<span data-ttu-id="2406e-128">5 </span><span class="sxs-lookup"><span data-stu-id="2406e-128">5</span></span>|<span data-ttu-id="2406e-129">操作失败</span><span class="sxs-lookup"><span data-stu-id="2406e-129">Action failed</span></span>|
|<span data-ttu-id="2406e-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="2406e-130">notSupported</span></span>|<span data-ttu-id="2406e-131">6 </span><span class="sxs-lookup"><span data-stu-id="2406e-131">6</span></span>|<span data-ttu-id="2406e-132">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="2406e-132">Action is not supported.</span></span>|





