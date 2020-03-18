---
title: actionState 枚举类型
description: 设备上操作的状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 734fa5b7920c64ed2f649f78a2e81de068e3e0db
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772256"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b441c-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b441c-103">actionState enum type</span></span>

> <span data-ttu-id="b441c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b441c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b441c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b441c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b441c-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="b441c-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="b441c-107">成员</span><span class="sxs-lookup"><span data-stu-id="b441c-107">Members</span></span>
|<span data-ttu-id="b441c-108">成员</span><span class="sxs-lookup"><span data-stu-id="b441c-108">Member</span></span>|<span data-ttu-id="b441c-109">值</span><span class="sxs-lookup"><span data-stu-id="b441c-109">Value</span></span>|<span data-ttu-id="b441c-110">说明</span><span class="sxs-lookup"><span data-stu-id="b441c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b441c-111">无</span><span class="sxs-lookup"><span data-stu-id="b441c-111">none</span></span>|<span data-ttu-id="b441c-112">0</span><span class="sxs-lookup"><span data-stu-id="b441c-112">0</span></span>|<span data-ttu-id="b441c-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="b441c-113">Not a valid action state</span></span>|
|<span data-ttu-id="b441c-114">决</span><span class="sxs-lookup"><span data-stu-id="b441c-114">pending</span></span>|<span data-ttu-id="b441c-115">1</span><span class="sxs-lookup"><span data-stu-id="b441c-115">1</span></span>|<span data-ttu-id="b441c-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="b441c-116">Action is pending</span></span>|
|<span data-ttu-id="b441c-117">取消</span><span class="sxs-lookup"><span data-stu-id="b441c-117">canceled</span></span>|<span data-ttu-id="b441c-118">双面</span><span class="sxs-lookup"><span data-stu-id="b441c-118">2</span></span>|<span data-ttu-id="b441c-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="b441c-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="b441c-120">工作</span><span class="sxs-lookup"><span data-stu-id="b441c-120">active</span></span>|<span data-ttu-id="b441c-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b441c-121">3</span></span>|<span data-ttu-id="b441c-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="b441c-122">Action is active.</span></span>|
|<span data-ttu-id="b441c-123">done</span><span class="sxs-lookup"><span data-stu-id="b441c-123">done</span></span>|<span data-ttu-id="b441c-124">4 </span><span class="sxs-lookup"><span data-stu-id="b441c-124">4</span></span>|<span data-ttu-id="b441c-125">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="b441c-125">Action completed without errors.</span></span>|
|<span data-ttu-id="b441c-126">未能</span><span class="sxs-lookup"><span data-stu-id="b441c-126">failed</span></span>|<span data-ttu-id="b441c-127">5 </span><span class="sxs-lookup"><span data-stu-id="b441c-127">5</span></span>|<span data-ttu-id="b441c-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="b441c-128">Action failed</span></span>|
|<span data-ttu-id="b441c-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="b441c-129">notSupported</span></span>|<span data-ttu-id="b441c-130">6 </span><span class="sxs-lookup"><span data-stu-id="b441c-130">6</span></span>|<span data-ttu-id="b441c-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="b441c-131">Action is not supported.</span></span>|



