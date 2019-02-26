---
title: actionState 枚举类型
description: 设备上操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261486"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="2b740-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2b740-103">actionState enum type</span></span>

> <span data-ttu-id="2b740-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b740-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b740-105">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="2b740-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="2b740-106">成员</span><span class="sxs-lookup"><span data-stu-id="2b740-106">Members</span></span>
|<span data-ttu-id="2b740-107">成员</span><span class="sxs-lookup"><span data-stu-id="2b740-107">Member</span></span>|<span data-ttu-id="2b740-108">值</span><span class="sxs-lookup"><span data-stu-id="2b740-108">Value</span></span>|<span data-ttu-id="2b740-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b740-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b740-110">无</span><span class="sxs-lookup"><span data-stu-id="2b740-110">none</span></span>|<span data-ttu-id="2b740-111">0</span><span class="sxs-lookup"><span data-stu-id="2b740-111">0</span></span>|<span data-ttu-id="2b740-112">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="2b740-112">Not a valid action state</span></span>|
|<span data-ttu-id="2b740-113">决</span><span class="sxs-lookup"><span data-stu-id="2b740-113">pending</span></span>|<span data-ttu-id="2b740-114">1</span><span class="sxs-lookup"><span data-stu-id="2b740-114">1</span></span>|<span data-ttu-id="2b740-115">操作挂起</span><span class="sxs-lookup"><span data-stu-id="2b740-115">Action is pending</span></span>|
|<span data-ttu-id="2b740-116">取消</span><span class="sxs-lookup"><span data-stu-id="2b740-116">canceled</span></span>|<span data-ttu-id="2b740-117">双面</span><span class="sxs-lookup"><span data-stu-id="2b740-117">2</span></span>|<span data-ttu-id="2b740-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="2b740-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="2b740-119">工作</span><span class="sxs-lookup"><span data-stu-id="2b740-119">active</span></span>|<span data-ttu-id="2b740-120">第三章</span><span class="sxs-lookup"><span data-stu-id="2b740-120">3</span></span>|<span data-ttu-id="2b740-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="2b740-121">Action is active.</span></span>|
|<span data-ttu-id="2b740-122">done</span><span class="sxs-lookup"><span data-stu-id="2b740-122">done</span></span>|<span data-ttu-id="2b740-123">4</span><span class="sxs-lookup"><span data-stu-id="2b740-123">4</span></span>|<span data-ttu-id="2b740-124">操作已完成, 无错误。</span><span class="sxs-lookup"><span data-stu-id="2b740-124">Action completed without errors.</span></span>|
|<span data-ttu-id="2b740-125">failed</span><span class="sxs-lookup"><span data-stu-id="2b740-125">failed</span></span>|<span data-ttu-id="2b740-126">5</span><span class="sxs-lookup"><span data-stu-id="2b740-126">5</span></span>|<span data-ttu-id="2b740-127">操作失败</span><span class="sxs-lookup"><span data-stu-id="2b740-127">Action failed</span></span>|
|<span data-ttu-id="2b740-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="2b740-128">notSupported</span></span>|<span data-ttu-id="2b740-129">型</span><span class="sxs-lookup"><span data-stu-id="2b740-129">6</span></span>|<span data-ttu-id="2b740-130">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="2b740-130">Action is not supported.</span></span>|



