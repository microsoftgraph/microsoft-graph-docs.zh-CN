---
title: actionState 枚举类型
description: 设备上操作的状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6be5ce422664d5666fd5c76c3ce51ad8a9d798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027515"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="a7e83-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a7e83-103">actionState enum type</span></span>

> <span data-ttu-id="a7e83-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7e83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e83-105">设备上操作的状态</span><span class="sxs-lookup"><span data-stu-id="a7e83-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="a7e83-106">成员</span><span class="sxs-lookup"><span data-stu-id="a7e83-106">Members</span></span>
|<span data-ttu-id="a7e83-107">成员</span><span class="sxs-lookup"><span data-stu-id="a7e83-107">Member</span></span>|<span data-ttu-id="a7e83-108">值</span><span class="sxs-lookup"><span data-stu-id="a7e83-108">Value</span></span>|<span data-ttu-id="a7e83-109">说明</span><span class="sxs-lookup"><span data-stu-id="a7e83-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e83-110">无</span><span class="sxs-lookup"><span data-stu-id="a7e83-110">none</span></span>|<span data-ttu-id="a7e83-111">0</span><span class="sxs-lookup"><span data-stu-id="a7e83-111">0</span></span>|<span data-ttu-id="a7e83-112">操作状态无效</span><span class="sxs-lookup"><span data-stu-id="a7e83-112">Not a valid action state</span></span>|
|<span data-ttu-id="a7e83-113">决</span><span class="sxs-lookup"><span data-stu-id="a7e83-113">pending</span></span>|<span data-ttu-id="a7e83-114">1</span><span class="sxs-lookup"><span data-stu-id="a7e83-114">1</span></span>|<span data-ttu-id="a7e83-115">操作挂起</span><span class="sxs-lookup"><span data-stu-id="a7e83-115">Action is pending</span></span>|
|<span data-ttu-id="a7e83-116">取消</span><span class="sxs-lookup"><span data-stu-id="a7e83-116">canceled</span></span>|<span data-ttu-id="a7e83-117">双面</span><span class="sxs-lookup"><span data-stu-id="a7e83-117">2</span></span>|<span data-ttu-id="a7e83-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="a7e83-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="a7e83-119">工作</span><span class="sxs-lookup"><span data-stu-id="a7e83-119">active</span></span>|<span data-ttu-id="a7e83-120">第三章</span><span class="sxs-lookup"><span data-stu-id="a7e83-120">3</span></span>|<span data-ttu-id="a7e83-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="a7e83-121">Action is active.</span></span>|
|<span data-ttu-id="a7e83-122">done</span><span class="sxs-lookup"><span data-stu-id="a7e83-122">done</span></span>|<span data-ttu-id="a7e83-123">4</span><span class="sxs-lookup"><span data-stu-id="a7e83-123">4</span></span>|<span data-ttu-id="a7e83-124">操作已完成, 无错误。</span><span class="sxs-lookup"><span data-stu-id="a7e83-124">Action completed without errors.</span></span>|
|<span data-ttu-id="a7e83-125">未能</span><span class="sxs-lookup"><span data-stu-id="a7e83-125">failed</span></span>|<span data-ttu-id="a7e83-126">5</span><span class="sxs-lookup"><span data-stu-id="a7e83-126">5</span></span>|<span data-ttu-id="a7e83-127">操作失败</span><span class="sxs-lookup"><span data-stu-id="a7e83-127">Action failed</span></span>|
|<span data-ttu-id="a7e83-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="a7e83-128">notSupported</span></span>|<span data-ttu-id="a7e83-129">型</span><span class="sxs-lookup"><span data-stu-id="a7e83-129">6</span></span>|<span data-ttu-id="a7e83-130">操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="a7e83-130">Action is not supported.</span></span>|



