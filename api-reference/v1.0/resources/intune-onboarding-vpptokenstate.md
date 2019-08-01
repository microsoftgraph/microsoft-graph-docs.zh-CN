---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c1effcc94eb7ed0929902c935c848e4610c1971b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037225"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="44ee7-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="44ee7-103">vppTokenState enum type</span></span>

> <span data-ttu-id="44ee7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44ee7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ee7-105">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="44ee7-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="44ee7-106">成员</span><span class="sxs-lookup"><span data-stu-id="44ee7-106">Members</span></span>
|<span data-ttu-id="44ee7-107">成员</span><span class="sxs-lookup"><span data-stu-id="44ee7-107">Member</span></span>|<span data-ttu-id="44ee7-108">值</span><span class="sxs-lookup"><span data-stu-id="44ee7-108">Value</span></span>|<span data-ttu-id="44ee7-109">说明</span><span class="sxs-lookup"><span data-stu-id="44ee7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ee7-110">unknown</span><span class="sxs-lookup"><span data-stu-id="44ee7-110">unknown</span></span>|<span data-ttu-id="44ee7-111">0</span><span class="sxs-lookup"><span data-stu-id="44ee7-111">0</span></span>|<span data-ttu-id="44ee7-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="44ee7-112">Default state.</span></span>|
|<span data-ttu-id="44ee7-113">有效</span><span class="sxs-lookup"><span data-stu-id="44ee7-113">valid</span></span>|<span data-ttu-id="44ee7-114">1</span><span class="sxs-lookup"><span data-stu-id="44ee7-114">1</span></span>|<span data-ttu-id="44ee7-115">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="44ee7-115">Token is valid.</span></span>|
|<span data-ttu-id="44ee7-116">期满</span><span class="sxs-lookup"><span data-stu-id="44ee7-116">expired</span></span>|<span data-ttu-id="44ee7-117">双面</span><span class="sxs-lookup"><span data-stu-id="44ee7-117">2</span></span>|<span data-ttu-id="44ee7-118">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="44ee7-118">Token is expired.</span></span>|
|<span data-ttu-id="44ee7-119">无效</span><span class="sxs-lookup"><span data-stu-id="44ee7-119">invalid</span></span>|<span data-ttu-id="44ee7-120">第三章</span><span class="sxs-lookup"><span data-stu-id="44ee7-120">3</span></span>|<span data-ttu-id="44ee7-121">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="44ee7-121">Token is invalid.</span></span>|
|<span data-ttu-id="44ee7-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="44ee7-122">assignedToExternalMDM</span></span>|<span data-ttu-id="44ee7-123">4</span><span class="sxs-lookup"><span data-stu-id="44ee7-123">4</span></span>|<span data-ttu-id="44ee7-124">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="44ee7-124">Token is managed by another MDM Service.</span></span>|



