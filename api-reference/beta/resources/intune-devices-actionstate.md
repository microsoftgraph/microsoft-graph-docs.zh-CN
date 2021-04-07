---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 99b7b189ed0e3f8a66eeaa4c099421b3b13e0989
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612137"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="753f1-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="753f1-103">actionState enum type</span></span>

<span data-ttu-id="753f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="753f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="753f1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="753f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="753f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="753f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="753f1-107">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="753f1-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="753f1-108">成员</span><span class="sxs-lookup"><span data-stu-id="753f1-108">Members</span></span>
|<span data-ttu-id="753f1-109">成员</span><span class="sxs-lookup"><span data-stu-id="753f1-109">Member</span></span>|<span data-ttu-id="753f1-110">值</span><span class="sxs-lookup"><span data-stu-id="753f1-110">Value</span></span>|<span data-ttu-id="753f1-111">Description</span><span class="sxs-lookup"><span data-stu-id="753f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="753f1-112">无</span><span class="sxs-lookup"><span data-stu-id="753f1-112">none</span></span>|<span data-ttu-id="753f1-113">0</span><span class="sxs-lookup"><span data-stu-id="753f1-113">0</span></span>|<span data-ttu-id="753f1-114">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="753f1-114">Not a valid action state</span></span>|
|<span data-ttu-id="753f1-115">pending</span><span class="sxs-lookup"><span data-stu-id="753f1-115">pending</span></span>|<span data-ttu-id="753f1-116">1</span><span class="sxs-lookup"><span data-stu-id="753f1-116">1</span></span>|<span data-ttu-id="753f1-117">操作挂起</span><span class="sxs-lookup"><span data-stu-id="753f1-117">Action is pending</span></span>|
|<span data-ttu-id="753f1-118">canceled</span><span class="sxs-lookup"><span data-stu-id="753f1-118">canceled</span></span>|<span data-ttu-id="753f1-119">2</span><span class="sxs-lookup"><span data-stu-id="753f1-119">2</span></span>|<span data-ttu-id="753f1-120">操作已取消。</span><span class="sxs-lookup"><span data-stu-id="753f1-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="753f1-121">active</span><span class="sxs-lookup"><span data-stu-id="753f1-121">active</span></span>|<span data-ttu-id="753f1-122">3</span><span class="sxs-lookup"><span data-stu-id="753f1-122">3</span></span>|<span data-ttu-id="753f1-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="753f1-123">Action is active.</span></span>|
|<span data-ttu-id="753f1-124">done</span><span class="sxs-lookup"><span data-stu-id="753f1-124">done</span></span>|<span data-ttu-id="753f1-125">4 </span><span class="sxs-lookup"><span data-stu-id="753f1-125">4</span></span>|<span data-ttu-id="753f1-126">操作已完成，没有错误。</span><span class="sxs-lookup"><span data-stu-id="753f1-126">Action completed without errors.</span></span>|
|<span data-ttu-id="753f1-127">failed</span><span class="sxs-lookup"><span data-stu-id="753f1-127">failed</span></span>|<span data-ttu-id="753f1-128">5 </span><span class="sxs-lookup"><span data-stu-id="753f1-128">5</span></span>|<span data-ttu-id="753f1-129">操作失败</span><span class="sxs-lookup"><span data-stu-id="753f1-129">Action failed</span></span>|
|<span data-ttu-id="753f1-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="753f1-130">notSupported</span></span>|<span data-ttu-id="753f1-131">6 </span><span class="sxs-lookup"><span data-stu-id="753f1-131">6</span></span>|<span data-ttu-id="753f1-132">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="753f1-132">Action is not supported.</span></span>|




