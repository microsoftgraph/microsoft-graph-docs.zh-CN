---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20890001aee15a56d5338964b931047033cf4a72
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030882"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="ff9d3-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ff9d3-103">complianceState enum type</span></span>

> <span data-ttu-id="ff9d3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff9d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff9d3-105">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="ff9d3-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="ff9d3-106">成员</span><span class="sxs-lookup"><span data-stu-id="ff9d3-106">Members</span></span>
|<span data-ttu-id="ff9d3-107">成员</span><span class="sxs-lookup"><span data-stu-id="ff9d3-107">Member</span></span>|<span data-ttu-id="ff9d3-108">值</span><span class="sxs-lookup"><span data-stu-id="ff9d3-108">Value</span></span>|<span data-ttu-id="ff9d3-109">说明</span><span class="sxs-lookup"><span data-stu-id="ff9d3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff9d3-110">unknown</span><span class="sxs-lookup"><span data-stu-id="ff9d3-110">unknown</span></span>|<span data-ttu-id="ff9d3-111">0</span><span class="sxs-lookup"><span data-stu-id="ff9d3-111">0</span></span>|<span data-ttu-id="ff9d3-112">陌生.</span><span class="sxs-lookup"><span data-stu-id="ff9d3-112">Unknown.</span></span>|
|<span data-ttu-id="ff9d3-113">合格</span><span class="sxs-lookup"><span data-stu-id="ff9d3-113">compliant</span></span>|<span data-ttu-id="ff9d3-114">1</span><span class="sxs-lookup"><span data-stu-id="ff9d3-114">1</span></span>|<span data-ttu-id="ff9d3-115">合格.</span><span class="sxs-lookup"><span data-stu-id="ff9d3-115">Compliant.</span></span>|
|<span data-ttu-id="ff9d3-116">合规</span><span class="sxs-lookup"><span data-stu-id="ff9d3-116">noncompliant</span></span>|<span data-ttu-id="ff9d3-117">双面</span><span class="sxs-lookup"><span data-stu-id="ff9d3-117">2</span></span>|<span data-ttu-id="ff9d3-118">设备不合规, 并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="ff9d3-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="ff9d3-119">冲突</span><span class="sxs-lookup"><span data-stu-id="ff9d3-119">conflict</span></span>|<span data-ttu-id="ff9d3-120">第三章</span><span class="sxs-lookup"><span data-stu-id="ff9d3-120">3</span></span>|<span data-ttu-id="ff9d3-121">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="ff9d3-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="ff9d3-122">error</span><span class="sxs-lookup"><span data-stu-id="ff9d3-122">error</span></span>|<span data-ttu-id="ff9d3-123">4</span><span class="sxs-lookup"><span data-stu-id="ff9d3-123">4</span></span>|<span data-ttu-id="ff9d3-124">错误。</span><span class="sxs-lookup"><span data-stu-id="ff9d3-124">Error.</span></span>|
|<span data-ttu-id="ff9d3-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="ff9d3-125">inGracePeriod</span></span>|<span data-ttu-id="ff9d3-126">254</span><span class="sxs-lookup"><span data-stu-id="ff9d3-126">254</span></span>|<span data-ttu-id="ff9d3-127">Device 不合规, 但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="ff9d3-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="ff9d3-128">configManager</span><span class="sxs-lookup"><span data-stu-id="ff9d3-128">configManager</span></span>|<span data-ttu-id="ff9d3-129">255</span><span class="sxs-lookup"><span data-stu-id="ff9d3-129">255</span></span>|<span data-ttu-id="ff9d3-130">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="ff9d3-130">Managed by Config Manager</span></span>|



