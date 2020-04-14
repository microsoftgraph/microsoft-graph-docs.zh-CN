---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 21979c33bc1dcc06b83f9169341aa67ca516f066
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446821"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="252f4-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="252f4-103">vppTokenState enum type</span></span>

<span data-ttu-id="252f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="252f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="252f4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="252f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="252f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="252f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="252f4-107">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="252f4-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="252f4-108">成员</span><span class="sxs-lookup"><span data-stu-id="252f4-108">Members</span></span>
|<span data-ttu-id="252f4-109">成员</span><span class="sxs-lookup"><span data-stu-id="252f4-109">Member</span></span>|<span data-ttu-id="252f4-110">值</span><span class="sxs-lookup"><span data-stu-id="252f4-110">Value</span></span>|<span data-ttu-id="252f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="252f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252f4-112">unknown</span><span class="sxs-lookup"><span data-stu-id="252f4-112">unknown</span></span>|<span data-ttu-id="252f4-113">0</span><span class="sxs-lookup"><span data-stu-id="252f4-113">0</span></span>|<span data-ttu-id="252f4-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="252f4-114">Default state.</span></span>|
|<span data-ttu-id="252f4-115">有效</span><span class="sxs-lookup"><span data-stu-id="252f4-115">valid</span></span>|<span data-ttu-id="252f4-116">1</span><span class="sxs-lookup"><span data-stu-id="252f4-116">1</span></span>|<span data-ttu-id="252f4-117">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="252f4-117">Token is valid.</span></span>|
|<span data-ttu-id="252f4-118">期满</span><span class="sxs-lookup"><span data-stu-id="252f4-118">expired</span></span>|<span data-ttu-id="252f4-119">双面</span><span class="sxs-lookup"><span data-stu-id="252f4-119">2</span></span>|<span data-ttu-id="252f4-120">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="252f4-120">Token is expired.</span></span>|
|<span data-ttu-id="252f4-121">无效</span><span class="sxs-lookup"><span data-stu-id="252f4-121">invalid</span></span>|<span data-ttu-id="252f4-122">第三章</span><span class="sxs-lookup"><span data-stu-id="252f4-122">3</span></span>|<span data-ttu-id="252f4-123">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="252f4-123">Token is invalid.</span></span>|
|<span data-ttu-id="252f4-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="252f4-124">assignedToExternalMDM</span></span>|<span data-ttu-id="252f4-125">4 </span><span class="sxs-lookup"><span data-stu-id="252f4-125">4</span></span>|<span data-ttu-id="252f4-126">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="252f4-126">Token is managed by another MDM Service.</span></span>|



