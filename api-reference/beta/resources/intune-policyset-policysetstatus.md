---
title: policySetStatus 枚举类型
description: 用于指定 PolicySet 状态的枚举。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 32ea9586ffee2ef112c58a1f88bdbdaefd654a04
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735155"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="a2446-103">policySetStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a2446-103">policySetStatus enum type</span></span>

<span data-ttu-id="a2446-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2446-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2446-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2446-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2446-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2446-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2446-107">用于指定 PolicySet 状态的枚举。</span><span class="sxs-lookup"><span data-stu-id="a2446-107">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="a2446-108">成员</span><span class="sxs-lookup"><span data-stu-id="a2446-108">Members</span></span>
|<span data-ttu-id="a2446-109">成员</span><span class="sxs-lookup"><span data-stu-id="a2446-109">Member</span></span>|<span data-ttu-id="a2446-110">值</span><span class="sxs-lookup"><span data-stu-id="a2446-110">Value</span></span>|<span data-ttu-id="a2446-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2446-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2446-112">unknown</span><span class="sxs-lookup"><span data-stu-id="a2446-112">unknown</span></span>|<span data-ttu-id="a2446-113">0</span><span class="sxs-lookup"><span data-stu-id="a2446-113">0</span></span>|<span data-ttu-id="a2446-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="a2446-114">Default Value.</span></span>|
|<span data-ttu-id="a2446-115">校验</span><span class="sxs-lookup"><span data-stu-id="a2446-115">validating</span></span>|<span data-ttu-id="a2446-116">1</span><span class="sxs-lookup"><span data-stu-id="a2446-116">1</span></span>|<span data-ttu-id="a2446-117">所有 PolicySet 项现在都在验证工作负荷的相应设置。</span><span class="sxs-lookup"><span data-stu-id="a2446-117">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="a2446-118">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="a2446-118">partialSuccess</span></span>|<span data-ttu-id="a2446-119">双面</span><span class="sxs-lookup"><span data-stu-id="a2446-119">2</span></span>|<span data-ttu-id="a2446-120">完成所有 PolicySet 项目的后过程，但出现故障。</span><span class="sxs-lookup"><span data-stu-id="a2446-120">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="a2446-121">success</span><span class="sxs-lookup"><span data-stu-id="a2446-121">success</span></span>|<span data-ttu-id="a2446-122">第三章</span><span class="sxs-lookup"><span data-stu-id="a2446-122">3</span></span>|<span data-ttu-id="a2446-123">部署所有 PolicySet 项目。</span><span class="sxs-lookup"><span data-stu-id="a2446-123">All PolicySet items are deployed.</span></span> <span data-ttu-id="a2446-124">并不意味着所有部署都成功。</span><span class="sxs-lookup"><span data-stu-id="a2446-124">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="a2446-125">error</span><span class="sxs-lookup"><span data-stu-id="a2446-125">error</span></span>|<span data-ttu-id="a2446-126">4 </span><span class="sxs-lookup"><span data-stu-id="a2446-126">4</span></span>|<span data-ttu-id="a2446-127">PolicySet 处理完全失败。</span><span class="sxs-lookup"><span data-stu-id="a2446-127">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="a2446-128">notAssigned</span><span class="sxs-lookup"><span data-stu-id="a2446-128">notAssigned</span></span>|<span data-ttu-id="a2446-129">5 </span><span class="sxs-lookup"><span data-stu-id="a2446-129">5</span></span>|<span data-ttu-id="a2446-130">PolicySet/PolicySetItem 未分配给任何组。</span><span class="sxs-lookup"><span data-stu-id="a2446-130">PolicySet/PolicySetItem is not assigned to any group.</span></span>|





