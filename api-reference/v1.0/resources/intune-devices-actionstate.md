---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d0544d0783109ca5f3616981c06ee330bfddea06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091325"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="0cce8-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0cce8-103">actionState enum type</span></span>

<span data-ttu-id="0cce8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cce8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cce8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cce8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cce8-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="0cce8-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="0cce8-107">成员</span><span class="sxs-lookup"><span data-stu-id="0cce8-107">Members</span></span>
|<span data-ttu-id="0cce8-108">成员</span><span class="sxs-lookup"><span data-stu-id="0cce8-108">Member</span></span>|<span data-ttu-id="0cce8-109">值</span><span class="sxs-lookup"><span data-stu-id="0cce8-109">Value</span></span>|<span data-ttu-id="0cce8-110">说明</span><span class="sxs-lookup"><span data-stu-id="0cce8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cce8-111">无</span><span class="sxs-lookup"><span data-stu-id="0cce8-111">none</span></span>|<span data-ttu-id="0cce8-112">0</span><span class="sxs-lookup"><span data-stu-id="0cce8-112">0</span></span>|<span data-ttu-id="0cce8-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="0cce8-113">Not a valid action state</span></span>|
|<span data-ttu-id="0cce8-114">决</span><span class="sxs-lookup"><span data-stu-id="0cce8-114">pending</span></span>|<span data-ttu-id="0cce8-115">1 </span><span class="sxs-lookup"><span data-stu-id="0cce8-115">1</span></span>|<span data-ttu-id="0cce8-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="0cce8-116">Action is pending</span></span>|
|<span data-ttu-id="0cce8-117">取消</span><span class="sxs-lookup"><span data-stu-id="0cce8-117">canceled</span></span>|<span data-ttu-id="0cce8-118">2 </span><span class="sxs-lookup"><span data-stu-id="0cce8-118">2</span></span>|<span data-ttu-id="0cce8-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="0cce8-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="0cce8-120">工作</span><span class="sxs-lookup"><span data-stu-id="0cce8-120">active</span></span>|<span data-ttu-id="0cce8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="0cce8-121">3</span></span>|<span data-ttu-id="0cce8-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="0cce8-122">Action is active.</span></span>|
|<span data-ttu-id="0cce8-123">done</span><span class="sxs-lookup"><span data-stu-id="0cce8-123">done</span></span>|<span data-ttu-id="0cce8-124">4 </span><span class="sxs-lookup"><span data-stu-id="0cce8-124">4</span></span>|<span data-ttu-id="0cce8-125">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="0cce8-125">Action completed without errors.</span></span>|
|<span data-ttu-id="0cce8-126">未能</span><span class="sxs-lookup"><span data-stu-id="0cce8-126">failed</span></span>|<span data-ttu-id="0cce8-127">5 </span><span class="sxs-lookup"><span data-stu-id="0cce8-127">5</span></span>|<span data-ttu-id="0cce8-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="0cce8-128">Action failed</span></span>|
|<span data-ttu-id="0cce8-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="0cce8-129">notSupported</span></span>|<span data-ttu-id="0cce8-130">6 </span><span class="sxs-lookup"><span data-stu-id="0cce8-130">6</span></span>|<span data-ttu-id="0cce8-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="0cce8-131">Action is not supported.</span></span>|









