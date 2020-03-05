---
title: actionState 枚举类型
description: 设备上操作的状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f4716f65c5405cf324d758ffd3c8bcf38d61b5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523770"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="1acd6-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1acd6-103">actionState enum type</span></span>

<span data-ttu-id="1acd6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1acd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1acd6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1acd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1acd6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1acd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1acd6-107">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="1acd6-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="1acd6-108">成员</span><span class="sxs-lookup"><span data-stu-id="1acd6-108">Members</span></span>
|<span data-ttu-id="1acd6-109">成员</span><span class="sxs-lookup"><span data-stu-id="1acd6-109">Member</span></span>|<span data-ttu-id="1acd6-110">值</span><span class="sxs-lookup"><span data-stu-id="1acd6-110">Value</span></span>|<span data-ttu-id="1acd6-111">说明</span><span class="sxs-lookup"><span data-stu-id="1acd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1acd6-112">无</span><span class="sxs-lookup"><span data-stu-id="1acd6-112">none</span></span>|<span data-ttu-id="1acd6-113">0</span><span class="sxs-lookup"><span data-stu-id="1acd6-113">0</span></span>|<span data-ttu-id="1acd6-114">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="1acd6-114">Not a valid action state</span></span>|
|<span data-ttu-id="1acd6-115">决</span><span class="sxs-lookup"><span data-stu-id="1acd6-115">pending</span></span>|<span data-ttu-id="1acd6-116">1 </span><span class="sxs-lookup"><span data-stu-id="1acd6-116">1</span></span>|<span data-ttu-id="1acd6-117">操作挂起</span><span class="sxs-lookup"><span data-stu-id="1acd6-117">Action is pending</span></span>|
|<span data-ttu-id="1acd6-118">取消</span><span class="sxs-lookup"><span data-stu-id="1acd6-118">canceled</span></span>|<span data-ttu-id="1acd6-119">2 </span><span class="sxs-lookup"><span data-stu-id="1acd6-119">2</span></span>|<span data-ttu-id="1acd6-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="1acd6-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="1acd6-121">工作</span><span class="sxs-lookup"><span data-stu-id="1acd6-121">active</span></span>|<span data-ttu-id="1acd6-122">3 </span><span class="sxs-lookup"><span data-stu-id="1acd6-122">3</span></span>|<span data-ttu-id="1acd6-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="1acd6-123">Action is active.</span></span>|
|<span data-ttu-id="1acd6-124">done</span><span class="sxs-lookup"><span data-stu-id="1acd6-124">done</span></span>|<span data-ttu-id="1acd6-125">4 </span><span class="sxs-lookup"><span data-stu-id="1acd6-125">4</span></span>|<span data-ttu-id="1acd6-126">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="1acd6-126">Action completed without errors.</span></span>|
|<span data-ttu-id="1acd6-127">未能</span><span class="sxs-lookup"><span data-stu-id="1acd6-127">failed</span></span>|<span data-ttu-id="1acd6-128">5 </span><span class="sxs-lookup"><span data-stu-id="1acd6-128">5</span></span>|<span data-ttu-id="1acd6-129">操作失败</span><span class="sxs-lookup"><span data-stu-id="1acd6-129">Action failed</span></span>|
|<span data-ttu-id="1acd6-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="1acd6-130">notSupported</span></span>|<span data-ttu-id="1acd6-131">6 </span><span class="sxs-lookup"><span data-stu-id="1acd6-131">6</span></span>|<span data-ttu-id="1acd6-132">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="1acd6-132">Action is not supported.</span></span>|



