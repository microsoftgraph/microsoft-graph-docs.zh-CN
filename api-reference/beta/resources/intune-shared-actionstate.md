---
title: actionState 枚举类型
description: 在设备上的操作的状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421611"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="ab14d-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab14d-103">actionState enum type</span></span>

> <span data-ttu-id="ab14d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ab14d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab14d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab14d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab14d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab14d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab14d-107">在设备上的操作的状态</span><span class="sxs-lookup"><span data-stu-id="ab14d-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="ab14d-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab14d-108">Members</span></span>
|<span data-ttu-id="ab14d-109">成员</span><span class="sxs-lookup"><span data-stu-id="ab14d-109">Member</span></span>|<span data-ttu-id="ab14d-110">值</span><span class="sxs-lookup"><span data-stu-id="ab14d-110">Value</span></span>|<span data-ttu-id="ab14d-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab14d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab14d-112">无</span><span class="sxs-lookup"><span data-stu-id="ab14d-112">none</span></span>|<span data-ttu-id="ab14d-113">0</span><span class="sxs-lookup"><span data-stu-id="ab14d-113">0</span></span>|<span data-ttu-id="ab14d-114">不是有效的操作状态</span><span class="sxs-lookup"><span data-stu-id="ab14d-114">Not a valid action state</span></span>|
|<span data-ttu-id="ab14d-115">挂起</span><span class="sxs-lookup"><span data-stu-id="ab14d-115">pending</span></span>|<span data-ttu-id="ab14d-116">1</span><span class="sxs-lookup"><span data-stu-id="ab14d-116">1</span></span>|<span data-ttu-id="ab14d-117">操作处于挂起状态</span><span class="sxs-lookup"><span data-stu-id="ab14d-117">Action is pending</span></span>|
|<span data-ttu-id="ab14d-118">取消此事件</span><span class="sxs-lookup"><span data-stu-id="ab14d-118">canceled</span></span>|<span data-ttu-id="ab14d-119">2</span><span class="sxs-lookup"><span data-stu-id="ab14d-119">2</span></span>|<span data-ttu-id="ab14d-120">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="ab14d-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="ab14d-121">活动</span><span class="sxs-lookup"><span data-stu-id="ab14d-121">active</span></span>|<span data-ttu-id="ab14d-122">3</span><span class="sxs-lookup"><span data-stu-id="ab14d-122">3</span></span>|<span data-ttu-id="ab14d-123">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="ab14d-123">Action is active.</span></span>|
|<span data-ttu-id="ab14d-124">done</span><span class="sxs-lookup"><span data-stu-id="ab14d-124">done</span></span>|<span data-ttu-id="ab14d-125">4</span><span class="sxs-lookup"><span data-stu-id="ab14d-125">4</span></span>|<span data-ttu-id="ab14d-126">没有错误完成的操作。</span><span class="sxs-lookup"><span data-stu-id="ab14d-126">Action completed without errors.</span></span>|
|<span data-ttu-id="ab14d-127">failed</span><span class="sxs-lookup"><span data-stu-id="ab14d-127">failed</span></span>|<span data-ttu-id="ab14d-128">5</span><span class="sxs-lookup"><span data-stu-id="ab14d-128">5</span></span>|<span data-ttu-id="ab14d-129">失败的操作</span><span class="sxs-lookup"><span data-stu-id="ab14d-129">Action failed</span></span>|
|<span data-ttu-id="ab14d-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="ab14d-130">notSupported</span></span>|<span data-ttu-id="ab14d-131">6</span><span class="sxs-lookup"><span data-stu-id="ab14d-131">6</span></span>|<span data-ttu-id="ab14d-132">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="ab14d-132">Action is not supported.</span></span>|




