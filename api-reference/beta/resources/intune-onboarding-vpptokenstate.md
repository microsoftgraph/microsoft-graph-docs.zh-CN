---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 415c3b0df84c6b15a0185876280b82c7e8ed3d20
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777381"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="940b9-103">vppTokenState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="940b9-103">vppTokenState enum type</span></span>

> <span data-ttu-id="940b9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="940b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="940b9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="940b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="940b9-106">与 Apple Volume Purchase Program 令牌关联的可能状态。</span><span class="sxs-lookup"><span data-stu-id="940b9-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="940b9-107">成员</span><span class="sxs-lookup"><span data-stu-id="940b9-107">Members</span></span>
|<span data-ttu-id="940b9-108">成员</span><span class="sxs-lookup"><span data-stu-id="940b9-108">Member</span></span>|<span data-ttu-id="940b9-109">值</span><span class="sxs-lookup"><span data-stu-id="940b9-109">Value</span></span>|<span data-ttu-id="940b9-110">说明</span><span class="sxs-lookup"><span data-stu-id="940b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940b9-111">unknown</span><span class="sxs-lookup"><span data-stu-id="940b9-111">unknown</span></span>|<span data-ttu-id="940b9-112">0</span><span class="sxs-lookup"><span data-stu-id="940b9-112">0</span></span>|<span data-ttu-id="940b9-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="940b9-113">Default state.</span></span>|
|<span data-ttu-id="940b9-114">有效</span><span class="sxs-lookup"><span data-stu-id="940b9-114">valid</span></span>|<span data-ttu-id="940b9-115">1</span><span class="sxs-lookup"><span data-stu-id="940b9-115">1</span></span>|<span data-ttu-id="940b9-116">令牌有效。</span><span class="sxs-lookup"><span data-stu-id="940b9-116">Token is valid.</span></span>|
|<span data-ttu-id="940b9-117">期满</span><span class="sxs-lookup"><span data-stu-id="940b9-117">expired</span></span>|<span data-ttu-id="940b9-118">双面</span><span class="sxs-lookup"><span data-stu-id="940b9-118">2</span></span>|<span data-ttu-id="940b9-119">令牌已过期。</span><span class="sxs-lookup"><span data-stu-id="940b9-119">Token is expired.</span></span>|
|<span data-ttu-id="940b9-120">无效</span><span class="sxs-lookup"><span data-stu-id="940b9-120">invalid</span></span>|<span data-ttu-id="940b9-121">第三章</span><span class="sxs-lookup"><span data-stu-id="940b9-121">3</span></span>|<span data-ttu-id="940b9-122">令牌无效。</span><span class="sxs-lookup"><span data-stu-id="940b9-122">Token is invalid.</span></span>|
|<span data-ttu-id="940b9-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="940b9-123">assignedToExternalMDM</span></span>|<span data-ttu-id="940b9-124">4 </span><span class="sxs-lookup"><span data-stu-id="940b9-124">4</span></span>|<span data-ttu-id="940b9-125">令牌由另一个 MDM 服务管理。</span><span class="sxs-lookup"><span data-stu-id="940b9-125">Token is managed by another MDM Service.</span></span>|



