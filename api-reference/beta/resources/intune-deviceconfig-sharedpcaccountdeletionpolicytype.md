---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 当共享 PC 上删除帐户可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7f51f76e6164c973b213eb53526d5961bb2b627
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861031"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="4a9c5-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4a9c5-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="4a9c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a9c5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a9c5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a9c5-107">当共享 PC 上删除帐户可能值。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="4a9c5-108">成员</span><span class="sxs-lookup"><span data-stu-id="4a9c5-108">Members</span></span>
|<span data-ttu-id="4a9c5-109">成员</span><span class="sxs-lookup"><span data-stu-id="4a9c5-109">Member</span></span>|<span data-ttu-id="4a9c5-110">值</span><span class="sxs-lookup"><span data-stu-id="4a9c5-110">Value</span></span>|<span data-ttu-id="4a9c5-111">Description</span><span class="sxs-lookup"><span data-stu-id="4a9c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a9c5-112">立即</span><span class="sxs-lookup"><span data-stu-id="4a9c5-112">immediate</span></span>|<span data-ttu-id="4a9c5-113">0</span><span class="sxs-lookup"><span data-stu-id="4a9c5-113">0</span></span>|<span data-ttu-id="4a9c5-114">立即删除。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-114">Delete immediately.</span></span>|
|<span data-ttu-id="4a9c5-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="4a9c5-115">diskSpaceThreshold</span></span>|<span data-ttu-id="4a9c5-116">1</span><span class="sxs-lookup"><span data-stu-id="4a9c5-116">1</span></span>|<span data-ttu-id="4a9c5-117">删除在磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="4a9c5-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="4a9c5-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="4a9c5-119">2</span><span class="sxs-lookup"><span data-stu-id="4a9c5-119">2</span></span>|<span data-ttu-id="4a9c5-120">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="4a9c5-120">Delete at disk space threshold or inactive threshold.</span></span>|





