---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9d94233233577d22a8c3661fb6e2ce82408d2a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139933"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="b9f8e-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b9f8e-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="b9f8e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9f8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f8e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9f8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f8e-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="b9f8e-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="b9f8e-107">成员</span><span class="sxs-lookup"><span data-stu-id="b9f8e-107">Members</span></span>
|<span data-ttu-id="b9f8e-108">成员</span><span class="sxs-lookup"><span data-stu-id="b9f8e-108">Member</span></span>|<span data-ttu-id="b9f8e-109">值</span><span class="sxs-lookup"><span data-stu-id="b9f8e-109">Value</span></span>|<span data-ttu-id="b9f8e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b9f8e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f8e-111">迫切</span><span class="sxs-lookup"><span data-stu-id="b9f8e-111">immediate</span></span>|<span data-ttu-id="b9f8e-112">0</span><span class="sxs-lookup"><span data-stu-id="b9f8e-112">0</span></span>|<span data-ttu-id="b9f8e-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="b9f8e-113">Delete immediately.</span></span>|
|<span data-ttu-id="b9f8e-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="b9f8e-114">diskSpaceThreshold</span></span>|<span data-ttu-id="b9f8e-115">1</span><span class="sxs-lookup"><span data-stu-id="b9f8e-115">1</span></span>|<span data-ttu-id="b9f8e-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="b9f8e-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="b9f8e-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="b9f8e-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="b9f8e-118">双面</span><span class="sxs-lookup"><span data-stu-id="b9f8e-118">2</span></span>|<span data-ttu-id="b9f8e-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="b9f8e-119">Delete at disk space threshold or inactive threshold.</span></span>|




