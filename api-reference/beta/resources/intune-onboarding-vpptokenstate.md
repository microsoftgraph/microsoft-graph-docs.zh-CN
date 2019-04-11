---
title: vppTokenState 枚举类型
description: 与 Apple volume Purchase Program 令牌关联的可能状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbc62b855035ebf68fefae3d628582b566804449
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781146"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="3c8e4-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3c8e4-103">vppTokenState enum type</span></span>

> <span data-ttu-id="3c8e4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c8e4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c8e4-106">与 Apple volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="3c8e4-107">成员</span><span class="sxs-lookup"><span data-stu-id="3c8e4-107">Members</span></span>
|<span data-ttu-id="3c8e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="3c8e4-108">Member</span></span>|<span data-ttu-id="3c8e4-109">值</span><span class="sxs-lookup"><span data-stu-id="3c8e4-109">Value</span></span>|<span data-ttu-id="3c8e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="3c8e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c8e4-111">unknown</span><span class="sxs-lookup"><span data-stu-id="3c8e4-111">unknown</span></span>|<span data-ttu-id="3c8e4-112">0</span><span class="sxs-lookup"><span data-stu-id="3c8e4-112">0</span></span>|<span data-ttu-id="3c8e4-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-113">Default state.</span></span>|
|<span data-ttu-id="3c8e4-114">有效</span><span class="sxs-lookup"><span data-stu-id="3c8e4-114">valid</span></span>|<span data-ttu-id="3c8e4-115">1</span><span class="sxs-lookup"><span data-stu-id="3c8e4-115">1</span></span>|<span data-ttu-id="3c8e4-116">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-116">Token is valid.</span></span>|
|<span data-ttu-id="3c8e4-117">期满</span><span class="sxs-lookup"><span data-stu-id="3c8e4-117">expired</span></span>|<span data-ttu-id="3c8e4-118">双面</span><span class="sxs-lookup"><span data-stu-id="3c8e4-118">2</span></span>|<span data-ttu-id="3c8e4-119">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-119">Token is expired.</span></span>|
|<span data-ttu-id="3c8e4-120">无效</span><span class="sxs-lookup"><span data-stu-id="3c8e4-120">invalid</span></span>|<span data-ttu-id="3c8e4-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3c8e4-121">3</span></span>|<span data-ttu-id="3c8e4-122">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-122">Token is invalid.</span></span>|
|<span data-ttu-id="3c8e4-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="3c8e4-123">assignedToExternalMDM</span></span>|<span data-ttu-id="3c8e4-124">4</span><span class="sxs-lookup"><span data-stu-id="3c8e4-124">4</span></span>|<span data-ttu-id="3c8e4-125">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="3c8e4-125">Token is managed by another MDM Service.</span></span>|





