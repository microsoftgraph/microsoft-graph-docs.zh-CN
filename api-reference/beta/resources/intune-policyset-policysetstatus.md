---
title: policySetStatus 枚举类型
description: 用于指定 PolicySet 状态的枚举。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a470e6c13bfd20ada920bbe2b471bfa96379092
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775147"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="e7fbd-103">policySetStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e7fbd-103">policySetStatus enum type</span></span>

> <span data-ttu-id="e7fbd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7fbd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7fbd-106">用于指定 PolicySet 状态的枚举。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-106">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="e7fbd-107">成员</span><span class="sxs-lookup"><span data-stu-id="e7fbd-107">Members</span></span>
|<span data-ttu-id="e7fbd-108">成员</span><span class="sxs-lookup"><span data-stu-id="e7fbd-108">Member</span></span>|<span data-ttu-id="e7fbd-109">值</span><span class="sxs-lookup"><span data-stu-id="e7fbd-109">Value</span></span>|<span data-ttu-id="e7fbd-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7fbd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7fbd-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e7fbd-111">unknown</span></span>|<span data-ttu-id="e7fbd-112">0</span><span class="sxs-lookup"><span data-stu-id="e7fbd-112">0</span></span>|<span data-ttu-id="e7fbd-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-113">Default Value.</span></span>|
|<span data-ttu-id="e7fbd-114">校验</span><span class="sxs-lookup"><span data-stu-id="e7fbd-114">validating</span></span>|<span data-ttu-id="e7fbd-115">1</span><span class="sxs-lookup"><span data-stu-id="e7fbd-115">1</span></span>|<span data-ttu-id="e7fbd-116">所有 PolicySet 项现在都在验证工作负荷的相应设置。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-116">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="e7fbd-117">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="e7fbd-117">partialSuccess</span></span>|<span data-ttu-id="e7fbd-118">双面</span><span class="sxs-lookup"><span data-stu-id="e7fbd-118">2</span></span>|<span data-ttu-id="e7fbd-119">完成所有 PolicySet 项目的后过程，但出现故障。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-119">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="e7fbd-120">success</span><span class="sxs-lookup"><span data-stu-id="e7fbd-120">success</span></span>|<span data-ttu-id="e7fbd-121">第三章</span><span class="sxs-lookup"><span data-stu-id="e7fbd-121">3</span></span>|<span data-ttu-id="e7fbd-122">部署所有 PolicySet 项目。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-122">All PolicySet items are deployed.</span></span> <span data-ttu-id="e7fbd-123">并不意味着所有部署都成功。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-123">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="e7fbd-124">error</span><span class="sxs-lookup"><span data-stu-id="e7fbd-124">error</span></span>|<span data-ttu-id="e7fbd-125">4 </span><span class="sxs-lookup"><span data-stu-id="e7fbd-125">4</span></span>|<span data-ttu-id="e7fbd-126">PolicySet 处理完全失败。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-126">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="e7fbd-127">notAssigned</span><span class="sxs-lookup"><span data-stu-id="e7fbd-127">notAssigned</span></span>|<span data-ttu-id="e7fbd-128">5 </span><span class="sxs-lookup"><span data-stu-id="e7fbd-128">5</span></span>|<span data-ttu-id="e7fbd-129">PolicySet/PolicySetItem 未分配给任何组。</span><span class="sxs-lookup"><span data-stu-id="e7fbd-129">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



