---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: faef244a196ae99a9ba82f4c5396db22b79be8b5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958513"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="ae1d8-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ae1d8-103">vppTokenState enum type</span></span>

> <span data-ttu-id="ae1d8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae1d8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae1d8-106">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="ae1d8-107">成员</span><span class="sxs-lookup"><span data-stu-id="ae1d8-107">Members</span></span>
|<span data-ttu-id="ae1d8-108">成员</span><span class="sxs-lookup"><span data-stu-id="ae1d8-108">Member</span></span>|<span data-ttu-id="ae1d8-109">值</span><span class="sxs-lookup"><span data-stu-id="ae1d8-109">Value</span></span>|<span data-ttu-id="ae1d8-110">说明</span><span class="sxs-lookup"><span data-stu-id="ae1d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1d8-111">unknown</span><span class="sxs-lookup"><span data-stu-id="ae1d8-111">unknown</span></span>|<span data-ttu-id="ae1d8-112">0</span><span class="sxs-lookup"><span data-stu-id="ae1d8-112">0</span></span>|<span data-ttu-id="ae1d8-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-113">Default state.</span></span>|
|<span data-ttu-id="ae1d8-114">有效</span><span class="sxs-lookup"><span data-stu-id="ae1d8-114">valid</span></span>|<span data-ttu-id="ae1d8-115">1</span><span class="sxs-lookup"><span data-stu-id="ae1d8-115">1</span></span>|<span data-ttu-id="ae1d8-116">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-116">Token is valid.</span></span>|
|<span data-ttu-id="ae1d8-117">期满</span><span class="sxs-lookup"><span data-stu-id="ae1d8-117">expired</span></span>|<span data-ttu-id="ae1d8-118">双面</span><span class="sxs-lookup"><span data-stu-id="ae1d8-118">2</span></span>|<span data-ttu-id="ae1d8-119">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-119">Token is expired.</span></span>|
|<span data-ttu-id="ae1d8-120">无效</span><span class="sxs-lookup"><span data-stu-id="ae1d8-120">invalid</span></span>|<span data-ttu-id="ae1d8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="ae1d8-121">3</span></span>|<span data-ttu-id="ae1d8-122">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-122">Token is invalid.</span></span>|
|<span data-ttu-id="ae1d8-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="ae1d8-123">assignedToExternalMDM</span></span>|<span data-ttu-id="ae1d8-124">4</span><span class="sxs-lookup"><span data-stu-id="ae1d8-124">4</span></span>|<span data-ttu-id="ae1d8-125">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="ae1d8-125">Token is managed by another MDM Service.</span></span>|





