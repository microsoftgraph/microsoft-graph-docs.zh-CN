---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fd6e9b2e30f7f3a57aa22ad2fa16a291df5d9b62
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472613"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="38a3f-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="38a3f-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="38a3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38a3f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38a3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a3f-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="38a3f-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="38a3f-107">成员</span><span class="sxs-lookup"><span data-stu-id="38a3f-107">Members</span></span>
|<span data-ttu-id="38a3f-108">成员</span><span class="sxs-lookup"><span data-stu-id="38a3f-108">Member</span></span>|<span data-ttu-id="38a3f-109">值</span><span class="sxs-lookup"><span data-stu-id="38a3f-109">Value</span></span>|<span data-ttu-id="38a3f-110">说明</span><span class="sxs-lookup"><span data-stu-id="38a3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a3f-111">迫切</span><span class="sxs-lookup"><span data-stu-id="38a3f-111">immediate</span></span>|<span data-ttu-id="38a3f-112">0</span><span class="sxs-lookup"><span data-stu-id="38a3f-112">0</span></span>|<span data-ttu-id="38a3f-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="38a3f-113">Delete immediately.</span></span>|
|<span data-ttu-id="38a3f-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="38a3f-114">diskSpaceThreshold</span></span>|<span data-ttu-id="38a3f-115">1</span><span class="sxs-lookup"><span data-stu-id="38a3f-115">1</span></span>|<span data-ttu-id="38a3f-116">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="38a3f-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="38a3f-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="38a3f-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="38a3f-118">双面</span><span class="sxs-lookup"><span data-stu-id="38a3f-118">2</span></span>|<span data-ttu-id="38a3f-119">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="38a3f-119">Delete at disk space threshold or inactive threshold.</span></span>|







