---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 45c695e1fb55617516905e25e4667a15b8f66c6c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787542"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="2325b-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2325b-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="2325b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2325b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2325b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2325b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2325b-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="2325b-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="2325b-107">成员</span><span class="sxs-lookup"><span data-stu-id="2325b-107">Members</span></span>
|<span data-ttu-id="2325b-108">成员</span><span class="sxs-lookup"><span data-stu-id="2325b-108">Member</span></span>|<span data-ttu-id="2325b-109">值</span><span class="sxs-lookup"><span data-stu-id="2325b-109">Value</span></span>|<span data-ttu-id="2325b-110">说明</span><span class="sxs-lookup"><span data-stu-id="2325b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2325b-111">迫切</span><span class="sxs-lookup"><span data-stu-id="2325b-111">immediate</span></span>|<span data-ttu-id="2325b-112">0</span><span class="sxs-lookup"><span data-stu-id="2325b-112">0</span></span>|<span data-ttu-id="2325b-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="2325b-113">Delete immediately.</span></span>|
|<span data-ttu-id="2325b-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="2325b-114">diskSpaceThreshold</span></span>|<span data-ttu-id="2325b-115">1</span><span class="sxs-lookup"><span data-stu-id="2325b-115">1</span></span>|<span data-ttu-id="2325b-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="2325b-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="2325b-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="2325b-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="2325b-118">双面</span><span class="sxs-lookup"><span data-stu-id="2325b-118">2</span></span>|<span data-ttu-id="2325b-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="2325b-119">Delete at disk space threshold or inactive threshold.</span></span>|



