---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 83370402104e4ebd42551262aaa98c109149e32e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067270"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fe158-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fe158-103">actionState enum type</span></span>

<span data-ttu-id="fe158-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe158-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe158-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe158-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe158-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe158-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe158-107">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="fe158-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="fe158-108">成员</span><span class="sxs-lookup"><span data-stu-id="fe158-108">Members</span></span>
|<span data-ttu-id="fe158-109">成员</span><span class="sxs-lookup"><span data-stu-id="fe158-109">Member</span></span>|<span data-ttu-id="fe158-110">值</span><span class="sxs-lookup"><span data-stu-id="fe158-110">Value</span></span>|<span data-ttu-id="fe158-111">说明</span><span class="sxs-lookup"><span data-stu-id="fe158-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe158-112">无</span><span class="sxs-lookup"><span data-stu-id="fe158-112">none</span></span>|<span data-ttu-id="fe158-113">0</span><span class="sxs-lookup"><span data-stu-id="fe158-113">0</span></span>|<span data-ttu-id="fe158-114">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="fe158-114">Not a valid action state</span></span>|
|<span data-ttu-id="fe158-115">决</span><span class="sxs-lookup"><span data-stu-id="fe158-115">pending</span></span>|<span data-ttu-id="fe158-116">1 </span><span class="sxs-lookup"><span data-stu-id="fe158-116">1</span></span>|<span data-ttu-id="fe158-117">操作挂起</span><span class="sxs-lookup"><span data-stu-id="fe158-117">Action is pending</span></span>|
|<span data-ttu-id="fe158-118">取消</span><span class="sxs-lookup"><span data-stu-id="fe158-118">canceled</span></span>|<span data-ttu-id="fe158-119">2 </span><span class="sxs-lookup"><span data-stu-id="fe158-119">2</span></span>|<span data-ttu-id="fe158-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="fe158-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="fe158-121">工作</span><span class="sxs-lookup"><span data-stu-id="fe158-121">active</span></span>|<span data-ttu-id="fe158-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fe158-122">3</span></span>|<span data-ttu-id="fe158-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fe158-123">Action is active.</span></span>|
|<span data-ttu-id="fe158-124">done</span><span class="sxs-lookup"><span data-stu-id="fe158-124">done</span></span>|<span data-ttu-id="fe158-125">4 </span><span class="sxs-lookup"><span data-stu-id="fe158-125">4</span></span>|<span data-ttu-id="fe158-126">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="fe158-126">Action completed without errors.</span></span>|
|<span data-ttu-id="fe158-127">未能</span><span class="sxs-lookup"><span data-stu-id="fe158-127">failed</span></span>|<span data-ttu-id="fe158-128">5 </span><span class="sxs-lookup"><span data-stu-id="fe158-128">5</span></span>|<span data-ttu-id="fe158-129">操作失败</span><span class="sxs-lookup"><span data-stu-id="fe158-129">Action failed</span></span>|
|<span data-ttu-id="fe158-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="fe158-130">notSupported</span></span>|<span data-ttu-id="fe158-131">6 </span><span class="sxs-lookup"><span data-stu-id="fe158-131">6</span></span>|<span data-ttu-id="fe158-132">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="fe158-132">Action is not supported.</span></span>|






