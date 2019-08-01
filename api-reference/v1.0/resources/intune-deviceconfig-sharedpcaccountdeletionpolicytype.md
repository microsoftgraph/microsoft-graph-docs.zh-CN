---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: da4f053301206143cf6ee617a6818ea57ddab3d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027823"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="ee3e3-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ee3e3-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="ee3e3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee3e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee3e3-105">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="ee3e3-105">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="ee3e3-106">成员</span><span class="sxs-lookup"><span data-stu-id="ee3e3-106">Members</span></span>
|<span data-ttu-id="ee3e3-107">成员</span><span class="sxs-lookup"><span data-stu-id="ee3e3-107">Member</span></span>|<span data-ttu-id="ee3e3-108">值</span><span class="sxs-lookup"><span data-stu-id="ee3e3-108">Value</span></span>|<span data-ttu-id="ee3e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee3e3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee3e3-110">迫切</span><span class="sxs-lookup"><span data-stu-id="ee3e3-110">immediate</span></span>|<span data-ttu-id="ee3e3-111">0</span><span class="sxs-lookup"><span data-stu-id="ee3e3-111">0</span></span>|<span data-ttu-id="ee3e3-112">立即删除。</span><span class="sxs-lookup"><span data-stu-id="ee3e3-112">Delete immediately.</span></span>|
|<span data-ttu-id="ee3e3-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="ee3e3-113">diskSpaceThreshold</span></span>|<span data-ttu-id="ee3e3-114">1</span><span class="sxs-lookup"><span data-stu-id="ee3e3-114">1</span></span>|<span data-ttu-id="ee3e3-115">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="ee3e3-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="ee3e3-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="ee3e3-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="ee3e3-117">双面</span><span class="sxs-lookup"><span data-stu-id="ee3e3-117">2</span></span>|<span data-ttu-id="ee3e3-118">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="ee3e3-118">Delete at disk space threshold or inactive threshold.</span></span>|



