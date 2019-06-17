---
title: actionState 枚举类型
description: 设备上操作的状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35fccdc65eec7781f38d366e31ddb1a626005169
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996223"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="f065d-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f065d-103">actionState enum type</span></span>

> <span data-ttu-id="f065d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f065d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f065d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f065d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f065d-106">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="f065d-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="f065d-107">成员</span><span class="sxs-lookup"><span data-stu-id="f065d-107">Members</span></span>
|<span data-ttu-id="f065d-108">成员</span><span class="sxs-lookup"><span data-stu-id="f065d-108">Member</span></span>|<span data-ttu-id="f065d-109">值</span><span class="sxs-lookup"><span data-stu-id="f065d-109">Value</span></span>|<span data-ttu-id="f065d-110">说明</span><span class="sxs-lookup"><span data-stu-id="f065d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f065d-111">无</span><span class="sxs-lookup"><span data-stu-id="f065d-111">none</span></span>|<span data-ttu-id="f065d-112">0</span><span class="sxs-lookup"><span data-stu-id="f065d-112">0</span></span>|<span data-ttu-id="f065d-113">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="f065d-113">Not a valid action state</span></span>|
|<span data-ttu-id="f065d-114">决</span><span class="sxs-lookup"><span data-stu-id="f065d-114">pending</span></span>|<span data-ttu-id="f065d-115">1</span><span class="sxs-lookup"><span data-stu-id="f065d-115">1</span></span>|<span data-ttu-id="f065d-116">操作挂起</span><span class="sxs-lookup"><span data-stu-id="f065d-116">Action is pending</span></span>|
|<span data-ttu-id="f065d-117">取消</span><span class="sxs-lookup"><span data-stu-id="f065d-117">canceled</span></span>|<span data-ttu-id="f065d-118">双面</span><span class="sxs-lookup"><span data-stu-id="f065d-118">2</span></span>|<span data-ttu-id="f065d-119">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="f065d-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="f065d-120">工作</span><span class="sxs-lookup"><span data-stu-id="f065d-120">active</span></span>|<span data-ttu-id="f065d-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f065d-121">3</span></span>|<span data-ttu-id="f065d-122">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="f065d-122">Action is active.</span></span>|
|<span data-ttu-id="f065d-123">done</span><span class="sxs-lookup"><span data-stu-id="f065d-123">done</span></span>|<span data-ttu-id="f065d-124">4</span><span class="sxs-lookup"><span data-stu-id="f065d-124">4</span></span>|<span data-ttu-id="f065d-125">操作已完成, 无错误。</span><span class="sxs-lookup"><span data-stu-id="f065d-125">Action completed without errors.</span></span>|
|<span data-ttu-id="f065d-126">未能</span><span class="sxs-lookup"><span data-stu-id="f065d-126">failed</span></span>|<span data-ttu-id="f065d-127">5</span><span class="sxs-lookup"><span data-stu-id="f065d-127">5</span></span>|<span data-ttu-id="f065d-128">操作失败</span><span class="sxs-lookup"><span data-stu-id="f065d-128">Action failed</span></span>|
|<span data-ttu-id="f065d-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="f065d-129">notSupported</span></span>|<span data-ttu-id="f065d-130">型</span><span class="sxs-lookup"><span data-stu-id="f065d-130">6</span></span>|<span data-ttu-id="f065d-131">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="f065d-131">Action is not supported.</span></span>|





