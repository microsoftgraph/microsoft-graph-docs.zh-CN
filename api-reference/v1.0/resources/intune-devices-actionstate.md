---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f805b39ac3954981c368ac79e566d3dc4fc218c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760214"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e167a-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e167a-103">actionState enum type</span></span>

<span data-ttu-id="e167a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e167a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e167a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e167a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e167a-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="e167a-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="e167a-107">成员</span><span class="sxs-lookup"><span data-stu-id="e167a-107">Members</span></span>
|<span data-ttu-id="e167a-108">成员</span><span class="sxs-lookup"><span data-stu-id="e167a-108">Member</span></span>|<span data-ttu-id="e167a-109">值</span><span class="sxs-lookup"><span data-stu-id="e167a-109">Value</span></span>|<span data-ttu-id="e167a-110">说明</span><span class="sxs-lookup"><span data-stu-id="e167a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e167a-111">无</span><span class="sxs-lookup"><span data-stu-id="e167a-111">none</span></span>|<span data-ttu-id="e167a-112">0</span><span class="sxs-lookup"><span data-stu-id="e167a-112">0</span></span>|<span data-ttu-id="e167a-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="e167a-113">Not a valid action state</span></span>|
|<span data-ttu-id="e167a-114">pending</span><span class="sxs-lookup"><span data-stu-id="e167a-114">pending</span></span>|<span data-ttu-id="e167a-115">1</span><span class="sxs-lookup"><span data-stu-id="e167a-115">1</span></span>|<span data-ttu-id="e167a-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="e167a-116">Action is pending</span></span>|
|<span data-ttu-id="e167a-117">canceled</span><span class="sxs-lookup"><span data-stu-id="e167a-117">canceled</span></span>|<span data-ttu-id="e167a-118">2</span><span class="sxs-lookup"><span data-stu-id="e167a-118">2</span></span>|<span data-ttu-id="e167a-119">操作已取消。</span><span class="sxs-lookup"><span data-stu-id="e167a-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="e167a-120">active</span><span class="sxs-lookup"><span data-stu-id="e167a-120">active</span></span>|<span data-ttu-id="e167a-121">3</span><span class="sxs-lookup"><span data-stu-id="e167a-121">3</span></span>|<span data-ttu-id="e167a-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="e167a-122">Action is active.</span></span>|
|<span data-ttu-id="e167a-123">done</span><span class="sxs-lookup"><span data-stu-id="e167a-123">done</span></span>|<span data-ttu-id="e167a-124">4 </span><span class="sxs-lookup"><span data-stu-id="e167a-124">4</span></span>|<span data-ttu-id="e167a-125">操作已完成，没有错误。</span><span class="sxs-lookup"><span data-stu-id="e167a-125">Action completed without errors.</span></span>|
|<span data-ttu-id="e167a-126">failed</span><span class="sxs-lookup"><span data-stu-id="e167a-126">failed</span></span>|<span data-ttu-id="e167a-127">5 </span><span class="sxs-lookup"><span data-stu-id="e167a-127">5</span></span>|<span data-ttu-id="e167a-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="e167a-128">Action failed</span></span>|
|<span data-ttu-id="e167a-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="e167a-129">notSupported</span></span>|<span data-ttu-id="e167a-130">6 </span><span class="sxs-lookup"><span data-stu-id="e167a-130">6</span></span>|<span data-ttu-id="e167a-131">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="e167a-131">Action is not supported.</span></span>|




