---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f38e2b1e99fb3d31064f1be63b1d9ae1618ee373
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451323"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="f7ff8-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f7ff8-103">actionState enum type</span></span>

<span data-ttu-id="f7ff8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ff8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7ff8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ff8-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="f7ff8-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="f7ff8-107">成员</span><span class="sxs-lookup"><span data-stu-id="f7ff8-107">Members</span></span>
|<span data-ttu-id="f7ff8-108">成员</span><span class="sxs-lookup"><span data-stu-id="f7ff8-108">Member</span></span>|<span data-ttu-id="f7ff8-109">值</span><span class="sxs-lookup"><span data-stu-id="f7ff8-109">Value</span></span>|<span data-ttu-id="f7ff8-110">说明</span><span class="sxs-lookup"><span data-stu-id="f7ff8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ff8-111">无</span><span class="sxs-lookup"><span data-stu-id="f7ff8-111">none</span></span>|<span data-ttu-id="f7ff8-112">0</span><span class="sxs-lookup"><span data-stu-id="f7ff8-112">0</span></span>|<span data-ttu-id="f7ff8-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="f7ff8-113">Not a valid action state</span></span>|
|<span data-ttu-id="f7ff8-114">决</span><span class="sxs-lookup"><span data-stu-id="f7ff8-114">pending</span></span>|<span data-ttu-id="f7ff8-115">1</span><span class="sxs-lookup"><span data-stu-id="f7ff8-115">1</span></span>|<span data-ttu-id="f7ff8-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="f7ff8-116">Action is pending</span></span>|
|<span data-ttu-id="f7ff8-117">取消</span><span class="sxs-lookup"><span data-stu-id="f7ff8-117">canceled</span></span>|<span data-ttu-id="f7ff8-118">双面</span><span class="sxs-lookup"><span data-stu-id="f7ff8-118">2</span></span>|<span data-ttu-id="f7ff8-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="f7ff8-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="f7ff8-120">工作</span><span class="sxs-lookup"><span data-stu-id="f7ff8-120">active</span></span>|<span data-ttu-id="f7ff8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f7ff8-121">3</span></span>|<span data-ttu-id="f7ff8-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="f7ff8-122">Action is active.</span></span>|
|<span data-ttu-id="f7ff8-123">done</span><span class="sxs-lookup"><span data-stu-id="f7ff8-123">done</span></span>|<span data-ttu-id="f7ff8-124">4 </span><span class="sxs-lookup"><span data-stu-id="f7ff8-124">4</span></span>|<span data-ttu-id="f7ff8-125">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="f7ff8-125">Action completed without errors.</span></span>|
|<span data-ttu-id="f7ff8-126">未能</span><span class="sxs-lookup"><span data-stu-id="f7ff8-126">failed</span></span>|<span data-ttu-id="f7ff8-127">5 </span><span class="sxs-lookup"><span data-stu-id="f7ff8-127">5</span></span>|<span data-ttu-id="f7ff8-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="f7ff8-128">Action failed</span></span>|
|<span data-ttu-id="f7ff8-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="f7ff8-129">notSupported</span></span>|<span data-ttu-id="f7ff8-130">6 </span><span class="sxs-lookup"><span data-stu-id="f7ff8-130">6</span></span>|<span data-ttu-id="f7ff8-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="f7ff8-131">Action is not supported.</span></span>|







