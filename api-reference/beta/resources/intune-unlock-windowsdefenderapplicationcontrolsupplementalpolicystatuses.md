---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f40b20966b5f260b9f59ae397499d4e7e63d5266
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523231"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="59647-103">windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型</span><span class="sxs-lookup"><span data-stu-id="59647-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

<span data-ttu-id="59647-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="59647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59647-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59647-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59647-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59647-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59647-107">各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。</span><span class="sxs-lookup"><span data-stu-id="59647-107">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="59647-108">成员</span><span class="sxs-lookup"><span data-stu-id="59647-108">Members</span></span>
|<span data-ttu-id="59647-109">成员</span><span class="sxs-lookup"><span data-stu-id="59647-109">Member</span></span>|<span data-ttu-id="59647-110">值</span><span class="sxs-lookup"><span data-stu-id="59647-110">Value</span></span>|<span data-ttu-id="59647-111">说明</span><span class="sxs-lookup"><span data-stu-id="59647-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59647-112">unknown</span><span class="sxs-lookup"><span data-stu-id="59647-112">unknown</span></span>|<span data-ttu-id="59647-113">0</span><span class="sxs-lookup"><span data-stu-id="59647-113">0</span></span>|<span data-ttu-id="59647-114">WindowsDefenderApplicationControl 补充策略的状态未知。</span><span class="sxs-lookup"><span data-stu-id="59647-114">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="59647-115">success</span><span class="sxs-lookup"><span data-stu-id="59647-115">success</span></span>|<span data-ttu-id="59647-116">1 </span><span class="sxs-lookup"><span data-stu-id="59647-116">1</span></span>|<span data-ttu-id="59647-117">WindowsDefenderApplicationControl 补充策略生效。</span><span class="sxs-lookup"><span data-stu-id="59647-117">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="59647-118">tokenError</span><span class="sxs-lookup"><span data-stu-id="59647-118">tokenError</span></span>|<span data-ttu-id="59647-119">2 </span><span class="sxs-lookup"><span data-stu-id="59647-119">2</span></span>|<span data-ttu-id="59647-120">WindowsDefenderApplicationControl 补充策略在结构上是正常的，但在授权令牌时发生错误。</span><span class="sxs-lookup"><span data-stu-id="59647-120">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="59647-121">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="59647-121">notAuthorizedByToken</span></span>|<span data-ttu-id="59647-122">3 </span><span class="sxs-lookup"><span data-stu-id="59647-122">3</span></span>|<span data-ttu-id="59647-123">令牌不授权此 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="59647-123">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="59647-124">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="59647-124">policyNotFound</span></span>|<span data-ttu-id="59647-125">4 </span><span class="sxs-lookup"><span data-stu-id="59647-125">4</span></span>|<span data-ttu-id="59647-126">找不到 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="59647-126">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



