---
title: vppTokenState 枚举类型
description: 与 Apple volume Purchase Program 令牌关联的可能状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbc62b855035ebf68fefae3d628582b566804449
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566421"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="e6bfc-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e6bfc-103">vppTokenState enum type</span></span>

> <span data-ttu-id="e6bfc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6bfc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6bfc-106">与 Apple volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="e6bfc-107">成员</span><span class="sxs-lookup"><span data-stu-id="e6bfc-107">Members</span></span>
|<span data-ttu-id="e6bfc-108">成员</span><span class="sxs-lookup"><span data-stu-id="e6bfc-108">Member</span></span>|<span data-ttu-id="e6bfc-109">值</span><span class="sxs-lookup"><span data-stu-id="e6bfc-109">Value</span></span>|<span data-ttu-id="e6bfc-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6bfc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6bfc-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e6bfc-111">unknown</span></span>|<span data-ttu-id="e6bfc-112">0</span><span class="sxs-lookup"><span data-stu-id="e6bfc-112">0</span></span>|<span data-ttu-id="e6bfc-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-113">Default state.</span></span>|
|<span data-ttu-id="e6bfc-114">有效</span><span class="sxs-lookup"><span data-stu-id="e6bfc-114">valid</span></span>|<span data-ttu-id="e6bfc-115">1</span><span class="sxs-lookup"><span data-stu-id="e6bfc-115">1</span></span>|<span data-ttu-id="e6bfc-116">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-116">Token is valid.</span></span>|
|<span data-ttu-id="e6bfc-117">期满</span><span class="sxs-lookup"><span data-stu-id="e6bfc-117">expired</span></span>|<span data-ttu-id="e6bfc-118">2 </span><span class="sxs-lookup"><span data-stu-id="e6bfc-118">2</span></span>|<span data-ttu-id="e6bfc-119">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-119">Token is expired.</span></span>|
|<span data-ttu-id="e6bfc-120">无效</span><span class="sxs-lookup"><span data-stu-id="e6bfc-120">invalid</span></span>|<span data-ttu-id="e6bfc-121">3 </span><span class="sxs-lookup"><span data-stu-id="e6bfc-121">3</span></span>|<span data-ttu-id="e6bfc-122">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-122">Token is invalid.</span></span>|
|<span data-ttu-id="e6bfc-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="e6bfc-123">assignedToExternalMDM</span></span>|<span data-ttu-id="e6bfc-124">4 </span><span class="sxs-lookup"><span data-stu-id="e6bfc-124">4</span></span>|<span data-ttu-id="e6bfc-125">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="e6bfc-125">Token is managed by another MDM Service.</span></span>|





