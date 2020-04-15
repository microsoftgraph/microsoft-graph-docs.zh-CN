---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 73dd5e2a60f2e73172d3fba853cc74f07ccfc5ee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453995"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="c5b2e-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c5b2e-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="c5b2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5b2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5b2e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5b2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5b2e-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="c5b2e-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="c5b2e-107">成员</span><span class="sxs-lookup"><span data-stu-id="c5b2e-107">Members</span></span>
|<span data-ttu-id="c5b2e-108">成员</span><span class="sxs-lookup"><span data-stu-id="c5b2e-108">Member</span></span>|<span data-ttu-id="c5b2e-109">值</span><span class="sxs-lookup"><span data-stu-id="c5b2e-109">Value</span></span>|<span data-ttu-id="c5b2e-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5b2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5b2e-111">无</span><span class="sxs-lookup"><span data-stu-id="c5b2e-111">none</span></span>|<span data-ttu-id="c5b2e-112">0</span><span class="sxs-lookup"><span data-stu-id="c5b2e-112">0</span></span>|<span data-ttu-id="c5b2e-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="c5b2e-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="c5b2e-114">unknown</span><span class="sxs-lookup"><span data-stu-id="c5b2e-114">unknown</span></span>|<span data-ttu-id="c5b2e-115">1</span><span class="sxs-lookup"><span data-stu-id="c5b2e-115">1</span></span>|<span data-ttu-id="c5b2e-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="c5b2e-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="c5b2e-117">支持</span><span class="sxs-lookup"><span data-stu-id="c5b2e-117">allowed</span></span>|<span data-ttu-id="c5b2e-118">双面</span><span class="sxs-lookup"><span data-stu-id="c5b2e-118">2</span></span>|<span data-ttu-id="c5b2e-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="c5b2e-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="c5b2e-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="c5b2e-120">blocked</span></span>|<span data-ttu-id="c5b2e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c5b2e-121">3</span></span>|<span data-ttu-id="c5b2e-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="c5b2e-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="c5b2e-123">隔离</span><span class="sxs-lookup"><span data-stu-id="c5b2e-123">quarantined</span></span>|<span data-ttu-id="c5b2e-124">4 </span><span class="sxs-lookup"><span data-stu-id="c5b2e-124">4</span></span>|<span data-ttu-id="c5b2e-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="c5b2e-125">Device is Quarantined in Exchange</span></span>|







