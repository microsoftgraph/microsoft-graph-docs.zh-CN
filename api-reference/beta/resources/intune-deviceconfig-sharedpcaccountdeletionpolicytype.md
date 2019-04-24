---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6db021476afdc47129fd677702bc6cc58af204fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464948"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="ae1a5-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ae1a5-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="ae1a5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae1a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae1a5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae1a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae1a5-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="ae1a5-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="ae1a5-107">成员</span><span class="sxs-lookup"><span data-stu-id="ae1a5-107">Members</span></span>
|<span data-ttu-id="ae1a5-108">成员</span><span class="sxs-lookup"><span data-stu-id="ae1a5-108">Member</span></span>|<span data-ttu-id="ae1a5-109">值</span><span class="sxs-lookup"><span data-stu-id="ae1a5-109">Value</span></span>|<span data-ttu-id="ae1a5-110">说明</span><span class="sxs-lookup"><span data-stu-id="ae1a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1a5-111">迫切</span><span class="sxs-lookup"><span data-stu-id="ae1a5-111">immediate</span></span>|<span data-ttu-id="ae1a5-112">0</span><span class="sxs-lookup"><span data-stu-id="ae1a5-112">0</span></span>|<span data-ttu-id="ae1a5-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="ae1a5-113">Delete immediately.</span></span>|
|<span data-ttu-id="ae1a5-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="ae1a5-114">diskSpaceThreshold</span></span>|<span data-ttu-id="ae1a5-115">1</span><span class="sxs-lookup"><span data-stu-id="ae1a5-115">1</span></span>|<span data-ttu-id="ae1a5-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="ae1a5-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="ae1a5-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="ae1a5-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="ae1a5-118">2 </span><span class="sxs-lookup"><span data-stu-id="ae1a5-118">2</span></span>|<span data-ttu-id="ae1a5-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="ae1a5-119">Delete at disk space threshold or inactive threshold.</span></span>|





