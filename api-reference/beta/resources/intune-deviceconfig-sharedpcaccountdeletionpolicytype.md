---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 12594665eb756f8d476f2a9eaab6c0c338407907
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049406"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="25dee-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="25dee-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="25dee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25dee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25dee-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25dee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25dee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25dee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25dee-107">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="25dee-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="25dee-108">成员</span><span class="sxs-lookup"><span data-stu-id="25dee-108">Members</span></span>
|<span data-ttu-id="25dee-109">成员</span><span class="sxs-lookup"><span data-stu-id="25dee-109">Member</span></span>|<span data-ttu-id="25dee-110">值</span><span class="sxs-lookup"><span data-stu-id="25dee-110">Value</span></span>|<span data-ttu-id="25dee-111">说明</span><span class="sxs-lookup"><span data-stu-id="25dee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25dee-112">迫切</span><span class="sxs-lookup"><span data-stu-id="25dee-112">immediate</span></span>|<span data-ttu-id="25dee-113">0</span><span class="sxs-lookup"><span data-stu-id="25dee-113">0</span></span>|<span data-ttu-id="25dee-114">立即删除。</span><span class="sxs-lookup"><span data-stu-id="25dee-114">Delete immediately.</span></span>|
|<span data-ttu-id="25dee-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="25dee-115">diskSpaceThreshold</span></span>|<span data-ttu-id="25dee-116">1 </span><span class="sxs-lookup"><span data-stu-id="25dee-116">1</span></span>|<span data-ttu-id="25dee-117">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="25dee-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="25dee-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="25dee-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="25dee-119">2 </span><span class="sxs-lookup"><span data-stu-id="25dee-119">2</span></span>|<span data-ttu-id="25dee-120">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="25dee-120">Delete at disk space threshold or inactive threshold.</span></span>|






