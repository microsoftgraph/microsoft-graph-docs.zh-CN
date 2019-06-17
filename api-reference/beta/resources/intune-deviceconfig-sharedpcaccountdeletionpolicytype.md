---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02c38abca522ec5ec0e50ffd3e4439b434fb9dfc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964281"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="2ac75-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2ac75-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="2ac75-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ac75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ac75-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ac75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac75-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="2ac75-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="2ac75-107">成员</span><span class="sxs-lookup"><span data-stu-id="2ac75-107">Members</span></span>
|<span data-ttu-id="2ac75-108">成员</span><span class="sxs-lookup"><span data-stu-id="2ac75-108">Member</span></span>|<span data-ttu-id="2ac75-109">值</span><span class="sxs-lookup"><span data-stu-id="2ac75-109">Value</span></span>|<span data-ttu-id="2ac75-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ac75-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac75-111">迫切</span><span class="sxs-lookup"><span data-stu-id="2ac75-111">immediate</span></span>|<span data-ttu-id="2ac75-112">0</span><span class="sxs-lookup"><span data-stu-id="2ac75-112">0</span></span>|<span data-ttu-id="2ac75-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="2ac75-113">Delete immediately.</span></span>|
|<span data-ttu-id="2ac75-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="2ac75-114">diskSpaceThreshold</span></span>|<span data-ttu-id="2ac75-115">1</span><span class="sxs-lookup"><span data-stu-id="2ac75-115">1</span></span>|<span data-ttu-id="2ac75-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="2ac75-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="2ac75-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="2ac75-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="2ac75-118">双面</span><span class="sxs-lookup"><span data-stu-id="2ac75-118">2</span></span>|<span data-ttu-id="2ac75-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="2ac75-119">Delete at disk space threshold or inactive threshold.</span></span>|





