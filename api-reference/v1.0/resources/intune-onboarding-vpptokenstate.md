---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f3eafcea71eed70fc96eee4a952ba8b44db2ebe6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360697"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="5e322-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5e322-103">vppTokenState enum type</span></span>

> <span data-ttu-id="5e322-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e322-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e322-105">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="5e322-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="5e322-106">成员</span><span class="sxs-lookup"><span data-stu-id="5e322-106">Members</span></span>
|<span data-ttu-id="5e322-107">成员</span><span class="sxs-lookup"><span data-stu-id="5e322-107">Member</span></span>|<span data-ttu-id="5e322-108">值</span><span class="sxs-lookup"><span data-stu-id="5e322-108">Value</span></span>|<span data-ttu-id="5e322-109">说明</span><span class="sxs-lookup"><span data-stu-id="5e322-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e322-110">unknown</span><span class="sxs-lookup"><span data-stu-id="5e322-110">unknown</span></span>|<span data-ttu-id="5e322-111">0</span><span class="sxs-lookup"><span data-stu-id="5e322-111">0</span></span>|<span data-ttu-id="5e322-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="5e322-112">Default state.</span></span>|
|<span data-ttu-id="5e322-113">有效</span><span class="sxs-lookup"><span data-stu-id="5e322-113">valid</span></span>|<span data-ttu-id="5e322-114">1</span><span class="sxs-lookup"><span data-stu-id="5e322-114">1</span></span>|<span data-ttu-id="5e322-115">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="5e322-115">Token is valid.</span></span>|
|<span data-ttu-id="5e322-116">期满</span><span class="sxs-lookup"><span data-stu-id="5e322-116">expired</span></span>|<span data-ttu-id="5e322-117">双面</span><span class="sxs-lookup"><span data-stu-id="5e322-117">2</span></span>|<span data-ttu-id="5e322-118">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="5e322-118">Token is expired.</span></span>|
|<span data-ttu-id="5e322-119">无效</span><span class="sxs-lookup"><span data-stu-id="5e322-119">invalid</span></span>|<span data-ttu-id="5e322-120">第三章</span><span class="sxs-lookup"><span data-stu-id="5e322-120">3</span></span>|<span data-ttu-id="5e322-121">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="5e322-121">Token is invalid.</span></span>|
|<span data-ttu-id="5e322-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="5e322-122">assignedToExternalMDM</span></span>|<span data-ttu-id="5e322-123">4</span><span class="sxs-lookup"><span data-stu-id="5e322-123">4</span></span>|<span data-ttu-id="5e322-124">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="5e322-124">Token is managed by another MDM Service.</span></span>|




