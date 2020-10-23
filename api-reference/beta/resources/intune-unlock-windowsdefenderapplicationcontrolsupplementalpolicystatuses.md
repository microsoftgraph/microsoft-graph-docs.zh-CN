---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5b56284a77fd390c265daab79e826f399464b9a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709752"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="4d32a-103">windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4d32a-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

<span data-ttu-id="4d32a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d32a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d32a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d32a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d32a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d32a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d32a-107">各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。</span><span class="sxs-lookup"><span data-stu-id="4d32a-107">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="4d32a-108">成员</span><span class="sxs-lookup"><span data-stu-id="4d32a-108">Members</span></span>
|<span data-ttu-id="4d32a-109">成员</span><span class="sxs-lookup"><span data-stu-id="4d32a-109">Member</span></span>|<span data-ttu-id="4d32a-110">值</span><span class="sxs-lookup"><span data-stu-id="4d32a-110">Value</span></span>|<span data-ttu-id="4d32a-111">说明</span><span class="sxs-lookup"><span data-stu-id="4d32a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d32a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="4d32a-112">unknown</span></span>|<span data-ttu-id="4d32a-113">0</span><span class="sxs-lookup"><span data-stu-id="4d32a-113">0</span></span>|<span data-ttu-id="4d32a-114">WindowsDefenderApplicationControl 补充策略的状态未知。</span><span class="sxs-lookup"><span data-stu-id="4d32a-114">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="4d32a-115">success</span><span class="sxs-lookup"><span data-stu-id="4d32a-115">success</span></span>|<span data-ttu-id="4d32a-116">1</span><span class="sxs-lookup"><span data-stu-id="4d32a-116">1</span></span>|<span data-ttu-id="4d32a-117">WindowsDefenderApplicationControl 补充策略生效。</span><span class="sxs-lookup"><span data-stu-id="4d32a-117">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="4d32a-118">tokenError</span><span class="sxs-lookup"><span data-stu-id="4d32a-118">tokenError</span></span>|<span data-ttu-id="4d32a-119">双面</span><span class="sxs-lookup"><span data-stu-id="4d32a-119">2</span></span>|<span data-ttu-id="4d32a-120">WindowsDefenderApplicationControl 补充策略在结构上是正常的，但在授权令牌时发生错误。</span><span class="sxs-lookup"><span data-stu-id="4d32a-120">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="4d32a-121">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="4d32a-121">notAuthorizedByToken</span></span>|<span data-ttu-id="4d32a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="4d32a-122">3</span></span>|<span data-ttu-id="4d32a-123">令牌不授权此 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="4d32a-123">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="4d32a-124">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="4d32a-124">policyNotFound</span></span>|<span data-ttu-id="4d32a-125">4 </span><span class="sxs-lookup"><span data-stu-id="4d32a-125">4</span></span>|<span data-ttu-id="4d32a-126">找不到 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="4d32a-126">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|





