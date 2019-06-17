---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35c110734078484f7bec5aac1ad31df0b66a0473
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983034"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="5af68-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5af68-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="5af68-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5af68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5af68-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5af68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5af68-106">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="5af68-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="5af68-107">成员</span><span class="sxs-lookup"><span data-stu-id="5af68-107">Members</span></span>
|<span data-ttu-id="5af68-108">成员</span><span class="sxs-lookup"><span data-stu-id="5af68-108">Member</span></span>|<span data-ttu-id="5af68-109">值</span><span class="sxs-lookup"><span data-stu-id="5af68-109">Value</span></span>|<span data-ttu-id="5af68-110">说明</span><span class="sxs-lookup"><span data-stu-id="5af68-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af68-111">无</span><span class="sxs-lookup"><span data-stu-id="5af68-111">none</span></span>|<span data-ttu-id="5af68-112">0</span><span class="sxs-lookup"><span data-stu-id="5af68-112">0</span></span>|<span data-ttu-id="5af68-113">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="5af68-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="5af68-114">unknown</span><span class="sxs-lookup"><span data-stu-id="5af68-114">unknown</span></span>|<span data-ttu-id="5af68-115">1</span><span class="sxs-lookup"><span data-stu-id="5af68-115">1</span></span>|<span data-ttu-id="5af68-116">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="5af68-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="5af68-117">支持</span><span class="sxs-lookup"><span data-stu-id="5af68-117">allowed</span></span>|<span data-ttu-id="5af68-118">双面</span><span class="sxs-lookup"><span data-stu-id="5af68-118">2</span></span>|<span data-ttu-id="5af68-119">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="5af68-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="5af68-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="5af68-120">blocked</span></span>|<span data-ttu-id="5af68-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5af68-121">3</span></span>|<span data-ttu-id="5af68-122">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="5af68-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="5af68-123">隔离</span><span class="sxs-lookup"><span data-stu-id="5af68-123">quarantined</span></span>|<span data-ttu-id="5af68-124">4</span><span class="sxs-lookup"><span data-stu-id="5af68-124">4</span></span>|<span data-ttu-id="5af68-125">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="5af68-125">Device is Quarantined in Exchange</span></span>|





