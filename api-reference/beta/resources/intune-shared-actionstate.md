---
title: actionState 枚举类型
description: 设备上操作的状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c213567b46c7aea2f91deae8bc8a27d4b0382c7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453178"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="ce698-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ce698-103">actionState enum type</span></span>

<span data-ttu-id="ce698-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce698-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce698-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce698-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce698-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce698-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce698-107">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="ce698-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="ce698-108">成员</span><span class="sxs-lookup"><span data-stu-id="ce698-108">Members</span></span>
|<span data-ttu-id="ce698-109">成员</span><span class="sxs-lookup"><span data-stu-id="ce698-109">Member</span></span>|<span data-ttu-id="ce698-110">值</span><span class="sxs-lookup"><span data-stu-id="ce698-110">Value</span></span>|<span data-ttu-id="ce698-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce698-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce698-112">无</span><span class="sxs-lookup"><span data-stu-id="ce698-112">none</span></span>|<span data-ttu-id="ce698-113">0</span><span class="sxs-lookup"><span data-stu-id="ce698-113">0</span></span>|<span data-ttu-id="ce698-114">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="ce698-114">Not a valid action state</span></span>|
|<span data-ttu-id="ce698-115">决</span><span class="sxs-lookup"><span data-stu-id="ce698-115">pending</span></span>|<span data-ttu-id="ce698-116">1</span><span class="sxs-lookup"><span data-stu-id="ce698-116">1</span></span>|<span data-ttu-id="ce698-117">操作挂起</span><span class="sxs-lookup"><span data-stu-id="ce698-117">Action is pending</span></span>|
|<span data-ttu-id="ce698-118">取消</span><span class="sxs-lookup"><span data-stu-id="ce698-118">canceled</span></span>|<span data-ttu-id="ce698-119">双面</span><span class="sxs-lookup"><span data-stu-id="ce698-119">2</span></span>|<span data-ttu-id="ce698-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="ce698-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="ce698-121">工作</span><span class="sxs-lookup"><span data-stu-id="ce698-121">active</span></span>|<span data-ttu-id="ce698-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ce698-122">3</span></span>|<span data-ttu-id="ce698-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="ce698-123">Action is active.</span></span>|
|<span data-ttu-id="ce698-124">done</span><span class="sxs-lookup"><span data-stu-id="ce698-124">done</span></span>|<span data-ttu-id="ce698-125">4 </span><span class="sxs-lookup"><span data-stu-id="ce698-125">4</span></span>|<span data-ttu-id="ce698-126">操作已完成，无错误。</span><span class="sxs-lookup"><span data-stu-id="ce698-126">Action completed without errors.</span></span>|
|<span data-ttu-id="ce698-127">未能</span><span class="sxs-lookup"><span data-stu-id="ce698-127">failed</span></span>|<span data-ttu-id="ce698-128">5 </span><span class="sxs-lookup"><span data-stu-id="ce698-128">5</span></span>|<span data-ttu-id="ce698-129">操作失败</span><span class="sxs-lookup"><span data-stu-id="ce698-129">Action failed</span></span>|
|<span data-ttu-id="ce698-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="ce698-130">notSupported</span></span>|<span data-ttu-id="ce698-131">6 </span><span class="sxs-lookup"><span data-stu-id="ce698-131">6</span></span>|<span data-ttu-id="ce698-132">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="ce698-132">Action is not supported.</span></span>|



