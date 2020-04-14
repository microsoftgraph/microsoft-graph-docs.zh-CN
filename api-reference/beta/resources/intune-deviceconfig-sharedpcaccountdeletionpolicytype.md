---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 539591836b9771b1b00288c33f08c3db754f322d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443348"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="3e93e-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3e93e-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="3e93e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e93e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e93e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e93e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e93e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e93e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e93e-107">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="3e93e-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="3e93e-108">成员</span><span class="sxs-lookup"><span data-stu-id="3e93e-108">Members</span></span>
|<span data-ttu-id="3e93e-109">成员</span><span class="sxs-lookup"><span data-stu-id="3e93e-109">Member</span></span>|<span data-ttu-id="3e93e-110">值</span><span class="sxs-lookup"><span data-stu-id="3e93e-110">Value</span></span>|<span data-ttu-id="3e93e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e93e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e93e-112">迫切</span><span class="sxs-lookup"><span data-stu-id="3e93e-112">immediate</span></span>|<span data-ttu-id="3e93e-113">0</span><span class="sxs-lookup"><span data-stu-id="3e93e-113">0</span></span>|<span data-ttu-id="3e93e-114">立即删除。</span><span class="sxs-lookup"><span data-stu-id="3e93e-114">Delete immediately.</span></span>|
|<span data-ttu-id="3e93e-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="3e93e-115">diskSpaceThreshold</span></span>|<span data-ttu-id="3e93e-116">1</span><span class="sxs-lookup"><span data-stu-id="3e93e-116">1</span></span>|<span data-ttu-id="3e93e-117">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="3e93e-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="3e93e-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="3e93e-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="3e93e-119">双面</span><span class="sxs-lookup"><span data-stu-id="3e93e-119">2</span></span>|<span data-ttu-id="3e93e-120">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="3e93e-120">Delete at disk space threshold or inactive threshold.</span></span>|



