---
title: complianceState 枚举类型
description: 合规性状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83f39e4c795d57b6bb5aa5633ed481963419e041
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983286"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="67373-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="67373-103">complianceState enum type</span></span>

> <span data-ttu-id="67373-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67373-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67373-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67373-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67373-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="67373-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="67373-107">成员</span><span class="sxs-lookup"><span data-stu-id="67373-107">Members</span></span>
|<span data-ttu-id="67373-108">成员</span><span class="sxs-lookup"><span data-stu-id="67373-108">Member</span></span>|<span data-ttu-id="67373-109">值</span><span class="sxs-lookup"><span data-stu-id="67373-109">Value</span></span>|<span data-ttu-id="67373-110">说明</span><span class="sxs-lookup"><span data-stu-id="67373-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67373-111">unknown</span><span class="sxs-lookup"><span data-stu-id="67373-111">unknown</span></span>|<span data-ttu-id="67373-112">0</span><span class="sxs-lookup"><span data-stu-id="67373-112">0</span></span>|<span data-ttu-id="67373-113">陌生.</span><span class="sxs-lookup"><span data-stu-id="67373-113">Unknown.</span></span>|
|<span data-ttu-id="67373-114">合格</span><span class="sxs-lookup"><span data-stu-id="67373-114">compliant</span></span>|<span data-ttu-id="67373-115">1</span><span class="sxs-lookup"><span data-stu-id="67373-115">1</span></span>|<span data-ttu-id="67373-116">合格.</span><span class="sxs-lookup"><span data-stu-id="67373-116">Compliant.</span></span>|
|<span data-ttu-id="67373-117">合规</span><span class="sxs-lookup"><span data-stu-id="67373-117">noncompliant</span></span>|<span data-ttu-id="67373-118">双面</span><span class="sxs-lookup"><span data-stu-id="67373-118">2</span></span>|<span data-ttu-id="67373-119">设备不合规, 并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="67373-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="67373-120">冲突</span><span class="sxs-lookup"><span data-stu-id="67373-120">conflict</span></span>|<span data-ttu-id="67373-121">第三章</span><span class="sxs-lookup"><span data-stu-id="67373-121">3</span></span>|<span data-ttu-id="67373-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="67373-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="67373-123">error</span><span class="sxs-lookup"><span data-stu-id="67373-123">error</span></span>|<span data-ttu-id="67373-124">4</span><span class="sxs-lookup"><span data-stu-id="67373-124">4</span></span>|<span data-ttu-id="67373-125">错误。</span><span class="sxs-lookup"><span data-stu-id="67373-125">Error.</span></span>|
|<span data-ttu-id="67373-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="67373-126">inGracePeriod</span></span>|<span data-ttu-id="67373-127">254</span><span class="sxs-lookup"><span data-stu-id="67373-127">254</span></span>|<span data-ttu-id="67373-128">Device 不合规, 但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="67373-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="67373-129">configManager</span><span class="sxs-lookup"><span data-stu-id="67373-129">configManager</span></span>|<span data-ttu-id="67373-130">255</span><span class="sxs-lookup"><span data-stu-id="67373-130">255</span></span>|<span data-ttu-id="67373-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="67373-131">Managed by Config Manager</span></span>|





