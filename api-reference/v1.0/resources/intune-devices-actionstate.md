---
title: actionState 枚举类型
description: 设备上操作的状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4cd21f0ac93e59d551400e87886e5bc871fd55c9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357085"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b7367-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b7367-103">actionState enum type</span></span>

> <span data-ttu-id="b7367-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7367-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7367-105">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="b7367-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="b7367-106">成员</span><span class="sxs-lookup"><span data-stu-id="b7367-106">Members</span></span>
|<span data-ttu-id="b7367-107">成员</span><span class="sxs-lookup"><span data-stu-id="b7367-107">Member</span></span>|<span data-ttu-id="b7367-108">值</span><span class="sxs-lookup"><span data-stu-id="b7367-108">Value</span></span>|<span data-ttu-id="b7367-109">说明</span><span class="sxs-lookup"><span data-stu-id="b7367-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7367-110">无</span><span class="sxs-lookup"><span data-stu-id="b7367-110">none</span></span>|<span data-ttu-id="b7367-111">0</span><span class="sxs-lookup"><span data-stu-id="b7367-111">0</span></span>|<span data-ttu-id="b7367-112">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="b7367-112">Not a valid action state</span></span>|
|<span data-ttu-id="b7367-113">决</span><span class="sxs-lookup"><span data-stu-id="b7367-113">pending</span></span>|<span data-ttu-id="b7367-114">1</span><span class="sxs-lookup"><span data-stu-id="b7367-114">1</span></span>|<span data-ttu-id="b7367-115">操作挂起</span><span class="sxs-lookup"><span data-stu-id="b7367-115">Action is pending</span></span>|
|<span data-ttu-id="b7367-116">取消</span><span class="sxs-lookup"><span data-stu-id="b7367-116">canceled</span></span>|<span data-ttu-id="b7367-117">双面</span><span class="sxs-lookup"><span data-stu-id="b7367-117">2</span></span>|<span data-ttu-id="b7367-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="b7367-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="b7367-119">工作</span><span class="sxs-lookup"><span data-stu-id="b7367-119">active</span></span>|<span data-ttu-id="b7367-120">第三章</span><span class="sxs-lookup"><span data-stu-id="b7367-120">3</span></span>|<span data-ttu-id="b7367-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="b7367-121">Action is active.</span></span>|
|<span data-ttu-id="b7367-122">done</span><span class="sxs-lookup"><span data-stu-id="b7367-122">done</span></span>|<span data-ttu-id="b7367-123">4</span><span class="sxs-lookup"><span data-stu-id="b7367-123">4</span></span>|<span data-ttu-id="b7367-124">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="b7367-124">Action completed without errors.</span></span>|
|<span data-ttu-id="b7367-125">未能</span><span class="sxs-lookup"><span data-stu-id="b7367-125">failed</span></span>|<span data-ttu-id="b7367-126">5</span><span class="sxs-lookup"><span data-stu-id="b7367-126">5</span></span>|<span data-ttu-id="b7367-127">操作失败</span><span class="sxs-lookup"><span data-stu-id="b7367-127">Action failed</span></span>|
|<span data-ttu-id="b7367-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="b7367-128">notSupported</span></span>|<span data-ttu-id="b7367-129">型</span><span class="sxs-lookup"><span data-stu-id="b7367-129">6</span></span>|<span data-ttu-id="b7367-130">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="b7367-130">Action is not supported.</span></span>|




