---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69f909f1bac3b33101d5e0e5515ad74588f46be2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449550"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="1ca38-103">windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1ca38-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

<span data-ttu-id="1ca38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ca38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ca38-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ca38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ca38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ca38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ca38-107">各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。</span><span class="sxs-lookup"><span data-stu-id="1ca38-107">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="1ca38-108">成员</span><span class="sxs-lookup"><span data-stu-id="1ca38-108">Members</span></span>
|<span data-ttu-id="1ca38-109">成员</span><span class="sxs-lookup"><span data-stu-id="1ca38-109">Member</span></span>|<span data-ttu-id="1ca38-110">值</span><span class="sxs-lookup"><span data-stu-id="1ca38-110">Value</span></span>|<span data-ttu-id="1ca38-111">说明</span><span class="sxs-lookup"><span data-stu-id="1ca38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ca38-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1ca38-112">unknown</span></span>|<span data-ttu-id="1ca38-113">0</span><span class="sxs-lookup"><span data-stu-id="1ca38-113">0</span></span>|<span data-ttu-id="1ca38-114">WindowsDefenderApplicationControl 补充策略的状态未知。</span><span class="sxs-lookup"><span data-stu-id="1ca38-114">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="1ca38-115">success</span><span class="sxs-lookup"><span data-stu-id="1ca38-115">success</span></span>|<span data-ttu-id="1ca38-116">1</span><span class="sxs-lookup"><span data-stu-id="1ca38-116">1</span></span>|<span data-ttu-id="1ca38-117">WindowsDefenderApplicationControl 补充策略生效。</span><span class="sxs-lookup"><span data-stu-id="1ca38-117">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="1ca38-118">tokenError</span><span class="sxs-lookup"><span data-stu-id="1ca38-118">tokenError</span></span>|<span data-ttu-id="1ca38-119">双面</span><span class="sxs-lookup"><span data-stu-id="1ca38-119">2</span></span>|<span data-ttu-id="1ca38-120">WindowsDefenderApplicationControl 补充策略在结构上是正常的，但在授权令牌时发生错误。</span><span class="sxs-lookup"><span data-stu-id="1ca38-120">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="1ca38-121">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="1ca38-121">notAuthorizedByToken</span></span>|<span data-ttu-id="1ca38-122">第三章</span><span class="sxs-lookup"><span data-stu-id="1ca38-122">3</span></span>|<span data-ttu-id="1ca38-123">令牌不授权此 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="1ca38-123">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="1ca38-124">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="1ca38-124">policyNotFound</span></span>|<span data-ttu-id="1ca38-125">4 </span><span class="sxs-lookup"><span data-stu-id="1ca38-125">4</span></span>|<span data-ttu-id="1ca38-126">找不到 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="1ca38-126">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



