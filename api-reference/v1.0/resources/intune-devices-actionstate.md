---
title: actionState 枚举类型
description: 设备上操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548458"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="c01b9-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c01b9-103">actionState enum type</span></span>

> <span data-ttu-id="c01b9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c01b9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c01b9-105">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="c01b9-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="c01b9-106">成员</span><span class="sxs-lookup"><span data-stu-id="c01b9-106">Members</span></span>
|<span data-ttu-id="c01b9-107">成员</span><span class="sxs-lookup"><span data-stu-id="c01b9-107">Member</span></span>|<span data-ttu-id="c01b9-108">值</span><span class="sxs-lookup"><span data-stu-id="c01b9-108">Value</span></span>|<span data-ttu-id="c01b9-109">说明</span><span class="sxs-lookup"><span data-stu-id="c01b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c01b9-110">无</span><span class="sxs-lookup"><span data-stu-id="c01b9-110">none</span></span>|<span data-ttu-id="c01b9-111">0</span><span class="sxs-lookup"><span data-stu-id="c01b9-111">0</span></span>|<span data-ttu-id="c01b9-112">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="c01b9-112">Not a valid action state</span></span>|
|<span data-ttu-id="c01b9-113">决</span><span class="sxs-lookup"><span data-stu-id="c01b9-113">pending</span></span>|<span data-ttu-id="c01b9-114">1</span><span class="sxs-lookup"><span data-stu-id="c01b9-114">1</span></span>|<span data-ttu-id="c01b9-115">操作挂起</span><span class="sxs-lookup"><span data-stu-id="c01b9-115">Action is pending</span></span>|
|<span data-ttu-id="c01b9-116">取消</span><span class="sxs-lookup"><span data-stu-id="c01b9-116">canceled</span></span>|<span data-ttu-id="c01b9-117">2 </span><span class="sxs-lookup"><span data-stu-id="c01b9-117">2</span></span>|<span data-ttu-id="c01b9-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="c01b9-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="c01b9-119">工作</span><span class="sxs-lookup"><span data-stu-id="c01b9-119">active</span></span>|<span data-ttu-id="c01b9-120">3 </span><span class="sxs-lookup"><span data-stu-id="c01b9-120">3</span></span>|<span data-ttu-id="c01b9-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="c01b9-121">Action is active.</span></span>|
|<span data-ttu-id="c01b9-122">done</span><span class="sxs-lookup"><span data-stu-id="c01b9-122">done</span></span>|<span data-ttu-id="c01b9-123">4 </span><span class="sxs-lookup"><span data-stu-id="c01b9-123">4</span></span>|<span data-ttu-id="c01b9-124">操作已完成, 无错误。</span><span class="sxs-lookup"><span data-stu-id="c01b9-124">Action completed without errors.</span></span>|
|<span data-ttu-id="c01b9-125">未能</span><span class="sxs-lookup"><span data-stu-id="c01b9-125">failed</span></span>|<span data-ttu-id="c01b9-126">5 </span><span class="sxs-lookup"><span data-stu-id="c01b9-126">5</span></span>|<span data-ttu-id="c01b9-127">操作失败</span><span class="sxs-lookup"><span data-stu-id="c01b9-127">Action failed</span></span>|
|<span data-ttu-id="c01b9-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="c01b9-128">notSupported</span></span>|<span data-ttu-id="c01b9-129">6 </span><span class="sxs-lookup"><span data-stu-id="c01b9-129">6</span></span>|<span data-ttu-id="c01b9-130">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="c01b9-130">Action is not supported.</span></span>|



