---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29357c5248aea78ffca8af464ecf4c3af17bdbc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172924"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="4e8cd-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4e8cd-103">complianceState enum type</span></span>

> <span data-ttu-id="4e8cd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e8cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e8cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e8cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e8cd-106">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="4e8cd-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="4e8cd-107">成员</span><span class="sxs-lookup"><span data-stu-id="4e8cd-107">Members</span></span>
|<span data-ttu-id="4e8cd-108">成员</span><span class="sxs-lookup"><span data-stu-id="4e8cd-108">Member</span></span>|<span data-ttu-id="4e8cd-109">值</span><span class="sxs-lookup"><span data-stu-id="4e8cd-109">Value</span></span>|<span data-ttu-id="4e8cd-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e8cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e8cd-111">unknown</span><span class="sxs-lookup"><span data-stu-id="4e8cd-111">unknown</span></span>|<span data-ttu-id="4e8cd-112">0</span><span class="sxs-lookup"><span data-stu-id="4e8cd-112">0</span></span>|<span data-ttu-id="4e8cd-113">陌生.</span><span class="sxs-lookup"><span data-stu-id="4e8cd-113">Unknown.</span></span>|
|<span data-ttu-id="4e8cd-114">合格</span><span class="sxs-lookup"><span data-stu-id="4e8cd-114">compliant</span></span>|<span data-ttu-id="4e8cd-115">1</span><span class="sxs-lookup"><span data-stu-id="4e8cd-115">1</span></span>|<span data-ttu-id="4e8cd-116">合格.</span><span class="sxs-lookup"><span data-stu-id="4e8cd-116">Compliant.</span></span>|
|<span data-ttu-id="4e8cd-117">合规</span><span class="sxs-lookup"><span data-stu-id="4e8cd-117">noncompliant</span></span>|<span data-ttu-id="4e8cd-118">双面</span><span class="sxs-lookup"><span data-stu-id="4e8cd-118">2</span></span>|<span data-ttu-id="4e8cd-119">设备不合规, 并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="4e8cd-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="4e8cd-120">冲突</span><span class="sxs-lookup"><span data-stu-id="4e8cd-120">conflict</span></span>|<span data-ttu-id="4e8cd-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4e8cd-121">3</span></span>|<span data-ttu-id="4e8cd-122">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="4e8cd-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="4e8cd-123">error</span><span class="sxs-lookup"><span data-stu-id="4e8cd-123">error</span></span>|<span data-ttu-id="4e8cd-124">4</span><span class="sxs-lookup"><span data-stu-id="4e8cd-124">4</span></span>|<span data-ttu-id="4e8cd-125">错误。</span><span class="sxs-lookup"><span data-stu-id="4e8cd-125">Error.</span></span>|
|<span data-ttu-id="4e8cd-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="4e8cd-126">inGracePeriod</span></span>|<span data-ttu-id="4e8cd-127">254</span><span class="sxs-lookup"><span data-stu-id="4e8cd-127">254</span></span>|<span data-ttu-id="4e8cd-128">Device 不合规, 但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="4e8cd-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="4e8cd-129">configManager</span><span class="sxs-lookup"><span data-stu-id="4e8cd-129">configManager</span></span>|<span data-ttu-id="4e8cd-130">255</span><span class="sxs-lookup"><span data-stu-id="4e8cd-130">255</span></span>|<span data-ttu-id="4e8cd-131">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="4e8cd-131">Managed by Config Manager</span></span>|




