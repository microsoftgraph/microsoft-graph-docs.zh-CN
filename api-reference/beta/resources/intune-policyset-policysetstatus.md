---
title: policySetStatus 枚举类型
description: 用于指定 PolicySet 状态的枚举。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a41e4f3dc01bd04c915dc4c883bae640b3e7683
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199955"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="f2e4d-103">policySetStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f2e4d-103">policySetStatus enum type</span></span>

> <span data-ttu-id="f2e4d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2e4d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e4d-106">用于指定 PolicySet 状态的枚举。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-106">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="f2e4d-107">成员</span><span class="sxs-lookup"><span data-stu-id="f2e4d-107">Members</span></span>
|<span data-ttu-id="f2e4d-108">成员</span><span class="sxs-lookup"><span data-stu-id="f2e4d-108">Member</span></span>|<span data-ttu-id="f2e4d-109">值</span><span class="sxs-lookup"><span data-stu-id="f2e4d-109">Value</span></span>|<span data-ttu-id="f2e4d-110">说明</span><span class="sxs-lookup"><span data-stu-id="f2e4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e4d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="f2e4d-111">unknown</span></span>|<span data-ttu-id="f2e4d-112">0</span><span class="sxs-lookup"><span data-stu-id="f2e4d-112">0</span></span>|<span data-ttu-id="f2e4d-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-113">Default Value.</span></span>|
|<span data-ttu-id="f2e4d-114">校验</span><span class="sxs-lookup"><span data-stu-id="f2e4d-114">validating</span></span>|<span data-ttu-id="f2e4d-115">1</span><span class="sxs-lookup"><span data-stu-id="f2e4d-115">1</span></span>|<span data-ttu-id="f2e4d-116">所有 PolicySet 项现在都在验证工作负荷的相应设置。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-116">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="f2e4d-117">partialSuccess</span><span class="sxs-lookup"><span data-stu-id="f2e4d-117">partialSuccess</span></span>|<span data-ttu-id="f2e4d-118">双面</span><span class="sxs-lookup"><span data-stu-id="f2e4d-118">2</span></span>|<span data-ttu-id="f2e4d-119">完成所有 PolicySet 项目的后过程，但出现故障。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-119">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="f2e4d-120">success</span><span class="sxs-lookup"><span data-stu-id="f2e4d-120">success</span></span>|<span data-ttu-id="f2e4d-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f2e4d-121">3</span></span>|<span data-ttu-id="f2e4d-122">部署所有 PolicySet 项目。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-122">All PolicySet items are deployed.</span></span> <span data-ttu-id="f2e4d-123">并不意味着所有部署都成功。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-123">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="f2e4d-124">error</span><span class="sxs-lookup"><span data-stu-id="f2e4d-124">error</span></span>|<span data-ttu-id="f2e4d-125">4</span><span class="sxs-lookup"><span data-stu-id="f2e4d-125">4</span></span>|<span data-ttu-id="f2e4d-126">PolicySet 处理完全失败。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-126">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="f2e4d-127">notAssigned</span><span class="sxs-lookup"><span data-stu-id="f2e4d-127">notAssigned</span></span>|<span data-ttu-id="f2e4d-128">5</span><span class="sxs-lookup"><span data-stu-id="f2e4d-128">5</span></span>|<span data-ttu-id="f2e4d-129">PolicySet/PolicySetItem 未分配给任何组。</span><span class="sxs-lookup"><span data-stu-id="f2e4d-129">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



