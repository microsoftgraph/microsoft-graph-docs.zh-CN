---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1999c999597d152396590e3faee6d7b472189500
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537655"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="1c5d9-103">windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1c5d9-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

> <span data-ttu-id="1c5d9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c5d9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c5d9-106">各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-106">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="1c5d9-107">成员</span><span class="sxs-lookup"><span data-stu-id="1c5d9-107">Members</span></span>
|<span data-ttu-id="1c5d9-108">成员</span><span class="sxs-lookup"><span data-stu-id="1c5d9-108">Member</span></span>|<span data-ttu-id="1c5d9-109">值</span><span class="sxs-lookup"><span data-stu-id="1c5d9-109">Value</span></span>|<span data-ttu-id="1c5d9-110">说明</span><span class="sxs-lookup"><span data-stu-id="1c5d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c5d9-111">unknown</span><span class="sxs-lookup"><span data-stu-id="1c5d9-111">unknown</span></span>|<span data-ttu-id="1c5d9-112">0</span><span class="sxs-lookup"><span data-stu-id="1c5d9-112">0</span></span>|<span data-ttu-id="1c5d9-113">WindowsDefenderApplicationControl 补充策略的状态未知。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-113">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="1c5d9-114">success</span><span class="sxs-lookup"><span data-stu-id="1c5d9-114">success</span></span>|<span data-ttu-id="1c5d9-115">1</span><span class="sxs-lookup"><span data-stu-id="1c5d9-115">1</span></span>|<span data-ttu-id="1c5d9-116">WindowsDefenderApplicationControl 补充策略生效。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-116">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="1c5d9-117">tokenError</span><span class="sxs-lookup"><span data-stu-id="1c5d9-117">tokenError</span></span>|<span data-ttu-id="1c5d9-118">双面</span><span class="sxs-lookup"><span data-stu-id="1c5d9-118">2</span></span>|<span data-ttu-id="1c5d9-119">WindowsDefenderApplicationControl 补充策略在结构上是正常的，但在授权令牌时发生错误。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-119">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="1c5d9-120">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="1c5d9-120">notAuthorizedByToken</span></span>|<span data-ttu-id="1c5d9-121">第三章</span><span class="sxs-lookup"><span data-stu-id="1c5d9-121">3</span></span>|<span data-ttu-id="1c5d9-122">令牌不授权此 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-122">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="1c5d9-123">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="1c5d9-123">policyNotFound</span></span>|<span data-ttu-id="1c5d9-124">4 </span><span class="sxs-lookup"><span data-stu-id="1c5d9-124">4</span></span>|<span data-ttu-id="1c5d9-125">找不到 WindowsDefenderApplicationControl 补充策略。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-125">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



