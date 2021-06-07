---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a3b4245ccf1a5a03d8b2142b65bfed69685de254
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751718"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="8a660-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8a660-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="8a660-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a660-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a660-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a660-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a660-106">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="8a660-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="8a660-107">成员</span><span class="sxs-lookup"><span data-stu-id="8a660-107">Members</span></span>
|<span data-ttu-id="8a660-108">成员</span><span class="sxs-lookup"><span data-stu-id="8a660-108">Member</span></span>|<span data-ttu-id="8a660-109">值</span><span class="sxs-lookup"><span data-stu-id="8a660-109">Value</span></span>|<span data-ttu-id="8a660-110">Description</span><span class="sxs-lookup"><span data-stu-id="8a660-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a660-111">immediate</span><span class="sxs-lookup"><span data-stu-id="8a660-111">immediate</span></span>|<span data-ttu-id="8a660-112">0</span><span class="sxs-lookup"><span data-stu-id="8a660-112">0</span></span>|<span data-ttu-id="8a660-113">立即删除。</span><span class="sxs-lookup"><span data-stu-id="8a660-113">Delete immediately.</span></span>|
|<span data-ttu-id="8a660-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="8a660-114">diskSpaceThreshold</span></span>|<span data-ttu-id="8a660-115">1</span><span class="sxs-lookup"><span data-stu-id="8a660-115">1</span></span>|<span data-ttu-id="8a660-116">达到磁盘空间阈值时删除。</span><span class="sxs-lookup"><span data-stu-id="8a660-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="8a660-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="8a660-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="8a660-118">2</span><span class="sxs-lookup"><span data-stu-id="8a660-118">2</span></span>|<span data-ttu-id="8a660-119">达到磁盘空间阈值或非活动阈值时删除。</span><span class="sxs-lookup"><span data-stu-id="8a660-119">Delete at disk space threshold or inactive threshold.</span></span>|




