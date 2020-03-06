---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4a60f207c36c8c17291d15789f33e391ea8c6d40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532337"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="fa42a-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fa42a-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="fa42a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa42a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa42a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa42a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa42a-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="fa42a-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="fa42a-107">成员</span><span class="sxs-lookup"><span data-stu-id="fa42a-107">Members</span></span>
|<span data-ttu-id="fa42a-108">成员</span><span class="sxs-lookup"><span data-stu-id="fa42a-108">Member</span></span>|<span data-ttu-id="fa42a-109">值</span><span class="sxs-lookup"><span data-stu-id="fa42a-109">Value</span></span>|<span data-ttu-id="fa42a-110">说明</span><span class="sxs-lookup"><span data-stu-id="fa42a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa42a-111">迫切</span><span class="sxs-lookup"><span data-stu-id="fa42a-111">immediate</span></span>|<span data-ttu-id="fa42a-112">0</span><span class="sxs-lookup"><span data-stu-id="fa42a-112">0</span></span>|<span data-ttu-id="fa42a-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="fa42a-113">Delete immediately.</span></span>|
|<span data-ttu-id="fa42a-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="fa42a-114">diskSpaceThreshold</span></span>|<span data-ttu-id="fa42a-115">1 </span><span class="sxs-lookup"><span data-stu-id="fa42a-115">1</span></span>|<span data-ttu-id="fa42a-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="fa42a-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="fa42a-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="fa42a-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="fa42a-118">2 </span><span class="sxs-lookup"><span data-stu-id="fa42a-118">2</span></span>|<span data-ttu-id="fa42a-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="fa42a-119">Delete at disk space threshold or inactive threshold.</span></span>|




