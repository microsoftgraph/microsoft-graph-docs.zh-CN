---
title: policySetStatus 枚举类型
description: 用于指定 PolicySet 状态的枚举。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b4fc37dd889edaa5a5050db3c162ec147d2573cf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448029"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="f3f08-103">policySetStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f3f08-103">policySetStatus enum type</span></span>

<span data-ttu-id="f3f08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3f08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3f08-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3f08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3f08-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3f08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3f08-107">用于指定 PolicySet 状态的枚举。</span><span class="sxs-lookup"><span data-stu-id="f3f08-107">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="f3f08-108">成员</span><span class="sxs-lookup"><span data-stu-id="f3f08-108">Members</span></span>
|<span data-ttu-id="f3f08-109">成员</span><span class="sxs-lookup"><span data-stu-id="f3f08-109">Member</span></span>|<span data-ttu-id="f3f08-110">值</span><span class="sxs-lookup"><span data-stu-id="f3f08-110">Value</span></span>|<span data-ttu-id="f3f08-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3f08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3f08-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f3f08-112">unknown</span></span>|<span data-ttu-id="f3f08-113">0</span><span class="sxs-lookup"><span data-stu-id="f3f08-113">0</span></span>|<span data-ttu-id="f3f08-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="f3f08-114">Default Value.</span></span>|
|<span data-ttu-id="f3f08-115">校验</span><span class="sxs-lookup"><span data-stu-id="f3f08-115">validating</span></span>|<span data-ttu-id="f3f08-116">1</span><span class="sxs-lookup"><span data-stu-id="f3f08-116">1</span></span>|<span data-ttu-id="f3f08-117">所有 PolicySet 项现在都在验证工作负荷的相应设置。</span><span class="sxs-lookup"><span data-stu-id="f3f08-117">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="f3f08-118">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="f3f08-118">partialSuccess</span></span>|<span data-ttu-id="f3f08-119">双面</span><span class="sxs-lookup"><span data-stu-id="f3f08-119">2</span></span>|<span data-ttu-id="f3f08-120">完成所有 PolicySet 项目的后过程，但出现故障。</span><span class="sxs-lookup"><span data-stu-id="f3f08-120">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="f3f08-121">success</span><span class="sxs-lookup"><span data-stu-id="f3f08-121">success</span></span>|<span data-ttu-id="f3f08-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f3f08-122">3</span></span>|<span data-ttu-id="f3f08-123">部署所有 PolicySet 项目。</span><span class="sxs-lookup"><span data-stu-id="f3f08-123">All PolicySet items are deployed.</span></span> <span data-ttu-id="f3f08-124">并不意味着所有部署都成功。</span><span class="sxs-lookup"><span data-stu-id="f3f08-124">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="f3f08-125">error</span><span class="sxs-lookup"><span data-stu-id="f3f08-125">error</span></span>|<span data-ttu-id="f3f08-126">4 </span><span class="sxs-lookup"><span data-stu-id="f3f08-126">4</span></span>|<span data-ttu-id="f3f08-127">PolicySet 处理完全失败。</span><span class="sxs-lookup"><span data-stu-id="f3f08-127">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="f3f08-128">notAssigned</span><span class="sxs-lookup"><span data-stu-id="f3f08-128">notAssigned</span></span>|<span data-ttu-id="f3f08-129">5 </span><span class="sxs-lookup"><span data-stu-id="f3f08-129">5</span></span>|<span data-ttu-id="f3f08-130">PolicySet/PolicySetItem 未分配给任何组。</span><span class="sxs-lookup"><span data-stu-id="f3f08-130">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



