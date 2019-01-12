---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 当共享 PC 上删除帐户可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5dc216d20becdc233bd1664250a958aa7208f1c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937626"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="98a8b-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="98a8b-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="98a8b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="98a8b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98a8b-105">当共享 PC 上删除帐户可能值。</span><span class="sxs-lookup"><span data-stu-id="98a8b-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="98a8b-106">成员</span><span class="sxs-lookup"><span data-stu-id="98a8b-106">Members</span></span>
|<span data-ttu-id="98a8b-107">成员</span><span class="sxs-lookup"><span data-stu-id="98a8b-107">Member</span></span>|<span data-ttu-id="98a8b-108">值</span><span class="sxs-lookup"><span data-stu-id="98a8b-108">Value</span></span>|<span data-ttu-id="98a8b-109">说明</span><span class="sxs-lookup"><span data-stu-id="98a8b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98a8b-110">立即</span><span class="sxs-lookup"><span data-stu-id="98a8b-110">immediate</span></span>|<span data-ttu-id="98a8b-111">0</span><span class="sxs-lookup"><span data-stu-id="98a8b-111">0</span></span>|<span data-ttu-id="98a8b-112">立即删除。</span><span class="sxs-lookup"><span data-stu-id="98a8b-112">Delete immediately.</span></span>|
|<span data-ttu-id="98a8b-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="98a8b-113">diskSpaceThreshold</span></span>|<span data-ttu-id="98a8b-114">1</span><span class="sxs-lookup"><span data-stu-id="98a8b-114">1</span></span>|<span data-ttu-id="98a8b-115">删除在磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="98a8b-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="98a8b-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="98a8b-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="98a8b-117">2</span><span class="sxs-lookup"><span data-stu-id="98a8b-117">2</span></span>|<span data-ttu-id="98a8b-118">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="98a8b-118">Delete at disk space threshold or inactive threshold.</span></span>|



