---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8fb006173b974ac902a99a2257ebbaeb52ea1d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066451"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="3cfa3-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3cfa3-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="3cfa3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfa3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cfa3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cfa3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cfa3-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="3cfa3-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="3cfa3-107">成员</span><span class="sxs-lookup"><span data-stu-id="3cfa3-107">Members</span></span>
|<span data-ttu-id="3cfa3-108">成员</span><span class="sxs-lookup"><span data-stu-id="3cfa3-108">Member</span></span>|<span data-ttu-id="3cfa3-109">值</span><span class="sxs-lookup"><span data-stu-id="3cfa3-109">Value</span></span>|<span data-ttu-id="3cfa3-110">说明</span><span class="sxs-lookup"><span data-stu-id="3cfa3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cfa3-111">迫切</span><span class="sxs-lookup"><span data-stu-id="3cfa3-111">immediate</span></span>|<span data-ttu-id="3cfa3-112">0</span><span class="sxs-lookup"><span data-stu-id="3cfa3-112">0</span></span>|<span data-ttu-id="3cfa3-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="3cfa3-113">Delete immediately.</span></span>|
|<span data-ttu-id="3cfa3-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="3cfa3-114">diskSpaceThreshold</span></span>|<span data-ttu-id="3cfa3-115">1 </span><span class="sxs-lookup"><span data-stu-id="3cfa3-115">1</span></span>|<span data-ttu-id="3cfa3-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="3cfa3-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="3cfa3-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="3cfa3-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="3cfa3-118">2 </span><span class="sxs-lookup"><span data-stu-id="3cfa3-118">2</span></span>|<span data-ttu-id="3cfa3-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="3cfa3-119">Delete at disk space threshold or inactive threshold.</span></span>|









