---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备交换访问状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b6058f35b86b1a8ae760fc8a3effb0f81f6571d4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356945"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="2b390-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2b390-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="2b390-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b390-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b390-105">设备交换访问状态。</span><span class="sxs-lookup"><span data-stu-id="2b390-105">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="2b390-106">成员</span><span class="sxs-lookup"><span data-stu-id="2b390-106">Members</span></span>
|<span data-ttu-id="2b390-107">成员</span><span class="sxs-lookup"><span data-stu-id="2b390-107">Member</span></span>|<span data-ttu-id="2b390-108">值</span><span class="sxs-lookup"><span data-stu-id="2b390-108">Value</span></span>|<span data-ttu-id="2b390-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b390-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b390-110">无</span><span class="sxs-lookup"><span data-stu-id="2b390-110">none</span></span>|<span data-ttu-id="2b390-111">0</span><span class="sxs-lookup"><span data-stu-id="2b390-111">0</span></span>|<span data-ttu-id="2b390-112">没有从 Exchange 中发现的访问状态</span><span class="sxs-lookup"><span data-stu-id="2b390-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="2b390-113">unknown</span><span class="sxs-lookup"><span data-stu-id="2b390-113">unknown</span></span>|<span data-ttu-id="2b390-114">1</span><span class="sxs-lookup"><span data-stu-id="2b390-114">1</span></span>|<span data-ttu-id="2b390-115">Exchange 的设备访问状态未知</span><span class="sxs-lookup"><span data-stu-id="2b390-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="2b390-116">支持</span><span class="sxs-lookup"><span data-stu-id="2b390-116">allowed</span></span>|<span data-ttu-id="2b390-117">双面</span><span class="sxs-lookup"><span data-stu-id="2b390-117">2</span></span>|<span data-ttu-id="2b390-118">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="2b390-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="2b390-119">堵塞</span><span class="sxs-lookup"><span data-stu-id="2b390-119">blocked</span></span>|<span data-ttu-id="2b390-120">第三章</span><span class="sxs-lookup"><span data-stu-id="2b390-120">3</span></span>|<span data-ttu-id="2b390-121">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="2b390-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="2b390-122">隔离</span><span class="sxs-lookup"><span data-stu-id="2b390-122">quarantined</span></span>|<span data-ttu-id="2b390-123">4</span><span class="sxs-lookup"><span data-stu-id="2b390-123">4</span></span>|<span data-ttu-id="2b390-124">Exchange 中的设备被隔离</span><span class="sxs-lookup"><span data-stu-id="2b390-124">Device is Quarantined in Exchange</span></span>|




