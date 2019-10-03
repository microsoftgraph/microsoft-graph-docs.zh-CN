---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0abed43fa5233e1e3a3f6a94ac020295e457f108
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367838"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="e5e12-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e5e12-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="e5e12-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5e12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5e12-105">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="e5e12-105">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="e5e12-106">成员</span><span class="sxs-lookup"><span data-stu-id="e5e12-106">Members</span></span>
|<span data-ttu-id="e5e12-107">成员</span><span class="sxs-lookup"><span data-stu-id="e5e12-107">Member</span></span>|<span data-ttu-id="e5e12-108">值</span><span class="sxs-lookup"><span data-stu-id="e5e12-108">Value</span></span>|<span data-ttu-id="e5e12-109">说明</span><span class="sxs-lookup"><span data-stu-id="e5e12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e12-110">迫切</span><span class="sxs-lookup"><span data-stu-id="e5e12-110">immediate</span></span>|<span data-ttu-id="e5e12-111">0</span><span class="sxs-lookup"><span data-stu-id="e5e12-111">0</span></span>|<span data-ttu-id="e5e12-112">立即删除。</span><span class="sxs-lookup"><span data-stu-id="e5e12-112">Delete immediately.</span></span>|
|<span data-ttu-id="e5e12-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="e5e12-113">diskSpaceThreshold</span></span>|<span data-ttu-id="e5e12-114">1</span><span class="sxs-lookup"><span data-stu-id="e5e12-114">1</span></span>|<span data-ttu-id="e5e12-115">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="e5e12-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="e5e12-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="e5e12-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="e5e12-117">双面</span><span class="sxs-lookup"><span data-stu-id="e5e12-117">2</span></span>|<span data-ttu-id="e5e12-118">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="e5e12-118">Delete at disk space threshold or inactive threshold.</span></span>|




