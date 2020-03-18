---
title: securityBaselineComplianceState 枚举类型
description: 安全基线合规性状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6042648d2e1d070c254eb617646fb15ba0ca0953
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785201"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="89b1a-103">securityBaselineComplianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89b1a-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="89b1a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89b1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89b1a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89b1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89b1a-106">安全基线合规性状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="89b1a-107">成员</span><span class="sxs-lookup"><span data-stu-id="89b1a-107">Members</span></span>
|<span data-ttu-id="89b1a-108">成员</span><span class="sxs-lookup"><span data-stu-id="89b1a-108">Member</span></span>|<span data-ttu-id="89b1a-109">值</span><span class="sxs-lookup"><span data-stu-id="89b1a-109">Value</span></span>|<span data-ttu-id="89b1a-110">说明</span><span class="sxs-lookup"><span data-stu-id="89b1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b1a-111">unknown</span><span class="sxs-lookup"><span data-stu-id="89b1a-111">unknown</span></span>|<span data-ttu-id="89b1a-112">0</span><span class="sxs-lookup"><span data-stu-id="89b1a-112">0</span></span>|<span data-ttu-id="89b1a-113">未知状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-113">Unknown state</span></span>|
|<span data-ttu-id="89b1a-114">安全</span><span class="sxs-lookup"><span data-stu-id="89b1a-114">secure</span></span>|<span data-ttu-id="89b1a-115">1</span><span class="sxs-lookup"><span data-stu-id="89b1a-115">1</span></span>|<span data-ttu-id="89b1a-116">安全状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-116">Secure state</span></span>|
|<span data-ttu-id="89b1a-117">notApplicable</span><span class="sxs-lookup"><span data-stu-id="89b1a-117">notApplicable</span></span>|<span data-ttu-id="89b1a-118">双面</span><span class="sxs-lookup"><span data-stu-id="89b1a-118">2</span></span>|<span data-ttu-id="89b1a-119">不适用的状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-119">Not applicable state</span></span>|
|<span data-ttu-id="89b1a-120">notSecure</span><span class="sxs-lookup"><span data-stu-id="89b1a-120">notSecure</span></span>|<span data-ttu-id="89b1a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="89b1a-121">3</span></span>|<span data-ttu-id="89b1a-122">不安全状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-122">Not secure state</span></span>|
|<span data-ttu-id="89b1a-123">error</span><span class="sxs-lookup"><span data-stu-id="89b1a-123">error</span></span>|<span data-ttu-id="89b1a-124">4 </span><span class="sxs-lookup"><span data-stu-id="89b1a-124">4</span></span>|<span data-ttu-id="89b1a-125">错误状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-125">Error state</span></span>|
|<span data-ttu-id="89b1a-126">冲突</span><span class="sxs-lookup"><span data-stu-id="89b1a-126">conflict</span></span>|<span data-ttu-id="89b1a-127">5 </span><span class="sxs-lookup"><span data-stu-id="89b1a-127">5</span></span>|<span data-ttu-id="89b1a-128">冲突状态</span><span class="sxs-lookup"><span data-stu-id="89b1a-128">Conflict state</span></span>|



