---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 309f3ead8ae67d3dda4c8c6f6d6a27a701f96d21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388351"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="28991-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="28991-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="28991-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28991-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28991-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28991-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28991-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28991-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28991-107">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="28991-107">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="28991-108">成员</span><span class="sxs-lookup"><span data-stu-id="28991-108">Members</span></span>
|<span data-ttu-id="28991-109">成员</span><span class="sxs-lookup"><span data-stu-id="28991-109">Member</span></span>|<span data-ttu-id="28991-110">值</span><span class="sxs-lookup"><span data-stu-id="28991-110">Value</span></span>|<span data-ttu-id="28991-111">说明</span><span class="sxs-lookup"><span data-stu-id="28991-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28991-112">无</span><span class="sxs-lookup"><span data-stu-id="28991-112">none</span></span>|<span data-ttu-id="28991-113">0</span><span class="sxs-lookup"><span data-stu-id="28991-113">0</span></span>|<span data-ttu-id="28991-114">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="28991-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="28991-115">unknown</span><span class="sxs-lookup"><span data-stu-id="28991-115">unknown</span></span>|<span data-ttu-id="28991-116">1</span><span class="sxs-lookup"><span data-stu-id="28991-116">1</span></span>|<span data-ttu-id="28991-117">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="28991-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="28991-118">支持</span><span class="sxs-lookup"><span data-stu-id="28991-118">allowed</span></span>|<span data-ttu-id="28991-119">双面</span><span class="sxs-lookup"><span data-stu-id="28991-119">2</span></span>|<span data-ttu-id="28991-120">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="28991-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="28991-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="28991-121">blocked</span></span>|<span data-ttu-id="28991-122">第三章</span><span class="sxs-lookup"><span data-stu-id="28991-122">3</span></span>|<span data-ttu-id="28991-123">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="28991-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="28991-124">隔离</span><span class="sxs-lookup"><span data-stu-id="28991-124">quarantined</span></span>|<span data-ttu-id="28991-125">4 </span><span class="sxs-lookup"><span data-stu-id="28991-125">4</span></span>|<span data-ttu-id="28991-126">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="28991-126">Device is Quarantined in Exchange</span></span>|



