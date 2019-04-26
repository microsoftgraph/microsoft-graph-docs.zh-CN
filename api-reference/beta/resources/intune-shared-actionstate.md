---
title: actionState 枚举类型
description: 设备上操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566316"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="146bb-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="146bb-103">actionState enum type</span></span>

> <span data-ttu-id="146bb-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="146bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="146bb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="146bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="146bb-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="146bb-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="146bb-107">成员</span><span class="sxs-lookup"><span data-stu-id="146bb-107">Members</span></span>
|<span data-ttu-id="146bb-108">成员</span><span class="sxs-lookup"><span data-stu-id="146bb-108">Member</span></span>|<span data-ttu-id="146bb-109">值</span><span class="sxs-lookup"><span data-stu-id="146bb-109">Value</span></span>|<span data-ttu-id="146bb-110">说明</span><span class="sxs-lookup"><span data-stu-id="146bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="146bb-111">无</span><span class="sxs-lookup"><span data-stu-id="146bb-111">none</span></span>|<span data-ttu-id="146bb-112">0</span><span class="sxs-lookup"><span data-stu-id="146bb-112">0</span></span>|<span data-ttu-id="146bb-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="146bb-113">Not a valid action state</span></span>|
|<span data-ttu-id="146bb-114">决</span><span class="sxs-lookup"><span data-stu-id="146bb-114">pending</span></span>|<span data-ttu-id="146bb-115">1</span><span class="sxs-lookup"><span data-stu-id="146bb-115">1</span></span>|<span data-ttu-id="146bb-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="146bb-116">Action is pending</span></span>|
|<span data-ttu-id="146bb-117">取消</span><span class="sxs-lookup"><span data-stu-id="146bb-117">canceled</span></span>|<span data-ttu-id="146bb-118">2 </span><span class="sxs-lookup"><span data-stu-id="146bb-118">2</span></span>|<span data-ttu-id="146bb-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="146bb-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="146bb-120">工作</span><span class="sxs-lookup"><span data-stu-id="146bb-120">active</span></span>|<span data-ttu-id="146bb-121">3 </span><span class="sxs-lookup"><span data-stu-id="146bb-121">3</span></span>|<span data-ttu-id="146bb-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="146bb-122">Action is active.</span></span>|
|<span data-ttu-id="146bb-123">done</span><span class="sxs-lookup"><span data-stu-id="146bb-123">done</span></span>|<span data-ttu-id="146bb-124">4 </span><span class="sxs-lookup"><span data-stu-id="146bb-124">4</span></span>|<span data-ttu-id="146bb-125">操作已完成, 无错误。</span><span class="sxs-lookup"><span data-stu-id="146bb-125">Action completed without errors.</span></span>|
|<span data-ttu-id="146bb-126">未能</span><span class="sxs-lookup"><span data-stu-id="146bb-126">failed</span></span>|<span data-ttu-id="146bb-127">5 </span><span class="sxs-lookup"><span data-stu-id="146bb-127">5</span></span>|<span data-ttu-id="146bb-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="146bb-128">Action failed</span></span>|
|<span data-ttu-id="146bb-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="146bb-129">notSupported</span></span>|<span data-ttu-id="146bb-130">6 </span><span class="sxs-lookup"><span data-stu-id="146bb-130">6</span></span>|<span data-ttu-id="146bb-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="146bb-131">Action is not supported.</span></span>|





