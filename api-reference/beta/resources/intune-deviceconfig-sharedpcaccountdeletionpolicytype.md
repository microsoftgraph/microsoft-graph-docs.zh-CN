---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90ece330d4d266c42a7a932d5962aaf1d85496e0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944710"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="91968-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="91968-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="91968-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91968-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91968-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91968-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91968-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="91968-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="91968-107">成员</span><span class="sxs-lookup"><span data-stu-id="91968-107">Members</span></span>
|<span data-ttu-id="91968-108">成员</span><span class="sxs-lookup"><span data-stu-id="91968-108">Member</span></span>|<span data-ttu-id="91968-109">值</span><span class="sxs-lookup"><span data-stu-id="91968-109">Value</span></span>|<span data-ttu-id="91968-110">说明</span><span class="sxs-lookup"><span data-stu-id="91968-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91968-111">迫切</span><span class="sxs-lookup"><span data-stu-id="91968-111">immediate</span></span>|<span data-ttu-id="91968-112">0</span><span class="sxs-lookup"><span data-stu-id="91968-112">0</span></span>|<span data-ttu-id="91968-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="91968-113">Delete immediately.</span></span>|
|<span data-ttu-id="91968-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="91968-114">diskSpaceThreshold</span></span>|<span data-ttu-id="91968-115">1</span><span class="sxs-lookup"><span data-stu-id="91968-115">1</span></span>|<span data-ttu-id="91968-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="91968-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="91968-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="91968-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="91968-118">双面</span><span class="sxs-lookup"><span data-stu-id="91968-118">2</span></span>|<span data-ttu-id="91968-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="91968-119">Delete at disk space threshold or inactive threshold.</span></span>|




