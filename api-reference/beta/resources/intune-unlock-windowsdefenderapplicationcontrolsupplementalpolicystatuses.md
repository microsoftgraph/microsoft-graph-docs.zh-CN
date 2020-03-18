---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 851bb0a5544a807b1ae73cac15dfa5f788271703
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764094"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="a39e2-103">windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a39e2-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

> <span data-ttu-id="a39e2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a39e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a39e2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a39e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a39e2-106">各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。</span><span class="sxs-lookup"><span data-stu-id="a39e2-106">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="a39e2-107">成员</span><span class="sxs-lookup"><span data-stu-id="a39e2-107">Members</span></span>
|<span data-ttu-id="a39e2-108">成员</span><span class="sxs-lookup"><span data-stu-id="a39e2-108">Member</span></span>|<span data-ttu-id="a39e2-109">值</span><span class="sxs-lookup"><span data-stu-id="a39e2-109">Value</span></span>|<span data-ttu-id="a39e2-110">说明</span><span class="sxs-lookup"><span data-stu-id="a39e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a39e2-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a39e2-111">unknown</span></span>|<span data-ttu-id="a39e2-112">0</span><span class="sxs-lookup"><span data-stu-id="a39e2-112">0</span></span>|<span data-ttu-id="a39e2-113">WindowsDefenderApplicationControl 补充策略的状态未知。</span><span class="sxs-lookup"><span data-stu-id="a39e2-113">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="a39e2-114">success</span><span class="sxs-lookup"><span data-stu-id="a39e2-114">success</span></span>|<span data-ttu-id="a39e2-115">1</span><span class="sxs-lookup"><span data-stu-id="a39e2-115">1</span></span>|<span data-ttu-id="a39e2-116">WindowsDefenderApplicationControl 补充策略生效。</span><span class="sxs-lookup"><span data-stu-id="a39e2-116">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="a39e2-117">tokenError</span><span class="sxs-lookup"><span data-stu-id="a39e2-117">tokenError</span></span>|<span data-ttu-id="a39e2-118">双面</span><span class="sxs-lookup"><span data-stu-id="a39e2-118">2</span></span>|<span data-ttu-id="a39e2-119">WindowsDefenderApplicationControl 补充策略在结构上是正常的，但在授权令牌时发生错误。</span><span class="sxs-lookup"><span data-stu-id="a39e2-119">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="a39e2-120">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="a39e2-120">notAuthorizedByToken</span></span>|<span data-ttu-id="a39e2-121">第三章</span><span class="sxs-lookup"><span data-stu-id="a39e2-121">3</span></span>|<span data-ttu-id="a39e2-122">令牌不授权此 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="a39e2-122">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="a39e2-123">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="a39e2-123">policyNotFound</span></span>|<span data-ttu-id="a39e2-124">4 </span><span class="sxs-lookup"><span data-stu-id="a39e2-124">4</span></span>|<span data-ttu-id="a39e2-125">找不到 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="a39e2-125">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



