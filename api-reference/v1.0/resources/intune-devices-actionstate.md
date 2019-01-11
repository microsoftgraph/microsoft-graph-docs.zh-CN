---
title: actionState 枚举类型
description: 在设备上的操作的状态
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0c05e283b94473a5c8c43498ff5bf1dd82da7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871937"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="ecf92-103">actionState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ecf92-103">actionState enum type</span></span>

> <span data-ttu-id="ecf92-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ecf92-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecf92-105">在设备上的操作的状态</span><span class="sxs-lookup"><span data-stu-id="ecf92-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="ecf92-106">成员</span><span class="sxs-lookup"><span data-stu-id="ecf92-106">Members</span></span>
|<span data-ttu-id="ecf92-107">成员</span><span class="sxs-lookup"><span data-stu-id="ecf92-107">Member</span></span>|<span data-ttu-id="ecf92-108">值</span><span class="sxs-lookup"><span data-stu-id="ecf92-108">Value</span></span>|<span data-ttu-id="ecf92-109">Description</span><span class="sxs-lookup"><span data-stu-id="ecf92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf92-110">无</span><span class="sxs-lookup"><span data-stu-id="ecf92-110">none</span></span>|<span data-ttu-id="ecf92-111">0</span><span class="sxs-lookup"><span data-stu-id="ecf92-111">0</span></span>|<span data-ttu-id="ecf92-112">不是有效的操作状态</span><span class="sxs-lookup"><span data-stu-id="ecf92-112">Not a valid action state</span></span>|
|<span data-ttu-id="ecf92-113">挂起</span><span class="sxs-lookup"><span data-stu-id="ecf92-113">pending</span></span>|<span data-ttu-id="ecf92-114">1</span><span class="sxs-lookup"><span data-stu-id="ecf92-114">1</span></span>|<span data-ttu-id="ecf92-115">操作处于挂起状态</span><span class="sxs-lookup"><span data-stu-id="ecf92-115">Action is pending</span></span>|
|<span data-ttu-id="ecf92-116">取消此事件</span><span class="sxs-lookup"><span data-stu-id="ecf92-116">canceled</span></span>|<span data-ttu-id="ecf92-117">2</span><span class="sxs-lookup"><span data-stu-id="ecf92-117">2</span></span>|<span data-ttu-id="ecf92-118">操作已被取消。</span><span class="sxs-lookup"><span data-stu-id="ecf92-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="ecf92-119">活动</span><span class="sxs-lookup"><span data-stu-id="ecf92-119">active</span></span>|<span data-ttu-id="ecf92-120">3</span><span class="sxs-lookup"><span data-stu-id="ecf92-120">3</span></span>|<span data-ttu-id="ecf92-121">操作处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="ecf92-121">Action is active.</span></span>|
|<span data-ttu-id="ecf92-122">done</span><span class="sxs-lookup"><span data-stu-id="ecf92-122">done</span></span>|<span data-ttu-id="ecf92-123">4</span><span class="sxs-lookup"><span data-stu-id="ecf92-123">4</span></span>|<span data-ttu-id="ecf92-124">没有错误完成的操作。</span><span class="sxs-lookup"><span data-stu-id="ecf92-124">Action completed without errors.</span></span>|
|<span data-ttu-id="ecf92-125">failed</span><span class="sxs-lookup"><span data-stu-id="ecf92-125">failed</span></span>|<span data-ttu-id="ecf92-126">5</span><span class="sxs-lookup"><span data-stu-id="ecf92-126">5</span></span>|<span data-ttu-id="ecf92-127">失败的操作</span><span class="sxs-lookup"><span data-stu-id="ecf92-127">Action failed</span></span>|
|<span data-ttu-id="ecf92-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="ecf92-128">notSupported</span></span>|<span data-ttu-id="ecf92-129">6</span><span class="sxs-lookup"><span data-stu-id="ecf92-129">6</span></span>|<span data-ttu-id="ecf92-130">不支持操作。</span><span class="sxs-lookup"><span data-stu-id="ecf92-130">Action is not supported.</span></span>|



