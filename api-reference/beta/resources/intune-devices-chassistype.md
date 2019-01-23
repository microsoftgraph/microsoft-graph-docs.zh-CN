---
title: chassisType 枚举类型
description: 机箱类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 29daba2a6e1c9aacf97b3b5b946d925c4163ea69
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422381"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="bb3e6-103">chassisType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bb3e6-103">chassisType enum type</span></span>

> <span data-ttu-id="bb3e6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb3e6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb3e6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb3e6-107">机箱类型。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-107">Chassis type.</span></span>

## <a name="members"></a><span data-ttu-id="bb3e6-108">成员</span><span class="sxs-lookup"><span data-stu-id="bb3e6-108">Members</span></span>
|<span data-ttu-id="bb3e6-109">成员</span><span class="sxs-lookup"><span data-stu-id="bb3e6-109">Member</span></span>|<span data-ttu-id="bb3e6-110">值</span><span class="sxs-lookup"><span data-stu-id="bb3e6-110">Value</span></span>|<span data-ttu-id="bb3e6-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb3e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb3e6-112">unknown</span><span class="sxs-lookup"><span data-stu-id="bb3e6-112">unknown</span></span>|<span data-ttu-id="bb3e6-113">0</span><span class="sxs-lookup"><span data-stu-id="bb3e6-113">0</span></span>|<span data-ttu-id="bb3e6-114">未知。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-114">Unknown.</span></span>|
|<span data-ttu-id="bb3e6-115">桌面</span><span class="sxs-lookup"><span data-stu-id="bb3e6-115">desktop</span></span>|<span data-ttu-id="bb3e6-116">1</span><span class="sxs-lookup"><span data-stu-id="bb3e6-116">1</span></span>|<span data-ttu-id="bb3e6-117">桌面。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-117">Desktop.</span></span>|
|<span data-ttu-id="bb3e6-118">便携式计算机</span><span class="sxs-lookup"><span data-stu-id="bb3e6-118">laptop</span></span>|<span data-ttu-id="bb3e6-119">2</span><span class="sxs-lookup"><span data-stu-id="bb3e6-119">2</span></span>|<span data-ttu-id="bb3e6-120">便携式计算机。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-120">Laptop.</span></span>|
|<span data-ttu-id="bb3e6-121">worksWorkstation</span><span class="sxs-lookup"><span data-stu-id="bb3e6-121">worksWorkstation</span></span>|<span data-ttu-id="bb3e6-122">3</span><span class="sxs-lookup"><span data-stu-id="bb3e6-122">3</span></span>|<span data-ttu-id="bb3e6-123">工作站。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-123">Workstation.</span></span>|
|<span data-ttu-id="bb3e6-124">enterpriseServer</span><span class="sxs-lookup"><span data-stu-id="bb3e6-124">enterpriseServer</span></span>|<span data-ttu-id="bb3e6-125">4</span><span class="sxs-lookup"><span data-stu-id="bb3e6-125">4</span></span>|<span data-ttu-id="bb3e6-126">企业服务器。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-126">Enterprise server.</span></span>|
|<span data-ttu-id="bb3e6-127">phone</span><span class="sxs-lookup"><span data-stu-id="bb3e6-127">phone</span></span>|<span data-ttu-id="bb3e6-128">100</span><span class="sxs-lookup"><span data-stu-id="bb3e6-128">100</span></span>|<span data-ttu-id="bb3e6-129">电话。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-129">Phone.</span></span>|
|<span data-ttu-id="bb3e6-130">平板电脑</span><span class="sxs-lookup"><span data-stu-id="bb3e6-130">tablet</span></span>|<span data-ttu-id="bb3e6-131">101</span><span class="sxs-lookup"><span data-stu-id="bb3e6-131">101</span></span>|<span data-ttu-id="bb3e6-132">移动平板电脑。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-132">Mobile tablet.</span></span>|
|<span data-ttu-id="bb3e6-133">mobileOther</span><span class="sxs-lookup"><span data-stu-id="bb3e6-133">mobileOther</span></span>|<span data-ttu-id="bb3e6-134">102</span><span class="sxs-lookup"><span data-stu-id="bb3e6-134">102</span></span>|<span data-ttu-id="bb3e6-135">其他移动。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-135">Other mobile.</span></span>|
|<span data-ttu-id="bb3e6-136">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="bb3e6-136">mobileUnknown</span></span>|<span data-ttu-id="bb3e6-137">103</span><span class="sxs-lookup"><span data-stu-id="bb3e6-137">103</span></span>|<span data-ttu-id="bb3e6-138">未知移动。</span><span class="sxs-lookup"><span data-stu-id="bb3e6-138">Unknown mobile.</span></span>|




