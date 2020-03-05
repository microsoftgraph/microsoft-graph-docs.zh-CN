---
title: actionState 枚举类型
description: 设备上操作的状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e11fc186dcfe16005e3ceaab5c6306f5893a8598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418165"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="f77d2-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f77d2-103">actionState enum type</span></span>

<span data-ttu-id="f77d2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f77d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f77d2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f77d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77d2-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="f77d2-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="f77d2-107">成员</span><span class="sxs-lookup"><span data-stu-id="f77d2-107">Members</span></span>
|<span data-ttu-id="f77d2-108">成员</span><span class="sxs-lookup"><span data-stu-id="f77d2-108">Member</span></span>|<span data-ttu-id="f77d2-109">值</span><span class="sxs-lookup"><span data-stu-id="f77d2-109">Value</span></span>|<span data-ttu-id="f77d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="f77d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77d2-111">无</span><span class="sxs-lookup"><span data-stu-id="f77d2-111">none</span></span>|<span data-ttu-id="f77d2-112">0</span><span class="sxs-lookup"><span data-stu-id="f77d2-112">0</span></span>|<span data-ttu-id="f77d2-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="f77d2-113">Not a valid action state</span></span>|
|<span data-ttu-id="f77d2-114">决</span><span class="sxs-lookup"><span data-stu-id="f77d2-114">pending</span></span>|<span data-ttu-id="f77d2-115">1 </span><span class="sxs-lookup"><span data-stu-id="f77d2-115">1</span></span>|<span data-ttu-id="f77d2-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="f77d2-116">Action is pending</span></span>|
|<span data-ttu-id="f77d2-117">取消</span><span class="sxs-lookup"><span data-stu-id="f77d2-117">canceled</span></span>|<span data-ttu-id="f77d2-118">2 </span><span class="sxs-lookup"><span data-stu-id="f77d2-118">2</span></span>|<span data-ttu-id="f77d2-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="f77d2-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="f77d2-120">工作</span><span class="sxs-lookup"><span data-stu-id="f77d2-120">active</span></span>|<span data-ttu-id="f77d2-121">3 </span><span class="sxs-lookup"><span data-stu-id="f77d2-121">3</span></span>|<span data-ttu-id="f77d2-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="f77d2-122">Action is active.</span></span>|
|<span data-ttu-id="f77d2-123">done</span><span class="sxs-lookup"><span data-stu-id="f77d2-123">done</span></span>|<span data-ttu-id="f77d2-124">4 </span><span class="sxs-lookup"><span data-stu-id="f77d2-124">4</span></span>|<span data-ttu-id="f77d2-125">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="f77d2-125">Action completed without errors.</span></span>|
|<span data-ttu-id="f77d2-126">未能</span><span class="sxs-lookup"><span data-stu-id="f77d2-126">failed</span></span>|<span data-ttu-id="f77d2-127">5 </span><span class="sxs-lookup"><span data-stu-id="f77d2-127">5</span></span>|<span data-ttu-id="f77d2-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="f77d2-128">Action failed</span></span>|
|<span data-ttu-id="f77d2-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="f77d2-129">notSupported</span></span>|<span data-ttu-id="f77d2-130">6 </span><span class="sxs-lookup"><span data-stu-id="f77d2-130">6</span></span>|<span data-ttu-id="f77d2-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="f77d2-131">Action is not supported.</span></span>|




