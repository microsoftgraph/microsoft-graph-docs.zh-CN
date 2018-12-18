---
title: chassisType 枚举类型
description: 机箱类型。
author: tfitzmac
ms.openlocfilehash: 2c65df4e324d186413936c44e611165b447df242
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327872"
---
# <a name="chassistype-enum-type"></a><span data-ttu-id="55a10-103">chassisType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55a10-103">chassisType enum type</span></span>

> <span data-ttu-id="55a10-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55a10-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55a10-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55a10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55a10-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55a10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55a10-107">机箱类型。</span><span class="sxs-lookup"><span data-stu-id="55a10-107">Chassis type.</span></span>
## <a name="members"></a><span data-ttu-id="55a10-108">成员</span><span class="sxs-lookup"><span data-stu-id="55a10-108">Members</span></span>
|<span data-ttu-id="55a10-109">成员</span><span class="sxs-lookup"><span data-stu-id="55a10-109">Member</span></span>|<span data-ttu-id="55a10-110">值</span><span class="sxs-lookup"><span data-stu-id="55a10-110">Value</span></span>|<span data-ttu-id="55a10-111">说明</span><span class="sxs-lookup"><span data-stu-id="55a10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55a10-112">unknown</span><span class="sxs-lookup"><span data-stu-id="55a10-112">unknown</span></span>|<span data-ttu-id="55a10-113">0</span><span class="sxs-lookup"><span data-stu-id="55a10-113">0</span></span>|<span data-ttu-id="55a10-114">未知。</span><span class="sxs-lookup"><span data-stu-id="55a10-114">Unknown.</span></span>|
|<span data-ttu-id="55a10-115">桌面</span><span class="sxs-lookup"><span data-stu-id="55a10-115">desktop</span></span>|<span data-ttu-id="55a10-116">1</span><span class="sxs-lookup"><span data-stu-id="55a10-116">1</span></span>|<span data-ttu-id="55a10-117">桌面。</span><span class="sxs-lookup"><span data-stu-id="55a10-117">Desktop.</span></span>|
|<span data-ttu-id="55a10-118">便携式计算机</span><span class="sxs-lookup"><span data-stu-id="55a10-118">laptop</span></span>|<span data-ttu-id="55a10-119">2</span><span class="sxs-lookup"><span data-stu-id="55a10-119">2</span></span>|<span data-ttu-id="55a10-120">便携式计算机。</span><span class="sxs-lookup"><span data-stu-id="55a10-120">Laptop.</span></span>|
|<span data-ttu-id="55a10-121">worksWorkstation</span><span class="sxs-lookup"><span data-stu-id="55a10-121">worksWorkstation</span></span>|<span data-ttu-id="55a10-122">3</span><span class="sxs-lookup"><span data-stu-id="55a10-122">3</span></span>|<span data-ttu-id="55a10-123">工作站。</span><span class="sxs-lookup"><span data-stu-id="55a10-123">Workstation.</span></span>|
|<span data-ttu-id="55a10-124">enterpriseServer</span><span class="sxs-lookup"><span data-stu-id="55a10-124">enterpriseServer</span></span>|<span data-ttu-id="55a10-125">4</span><span class="sxs-lookup"><span data-stu-id="55a10-125">4</span></span>|<span data-ttu-id="55a10-126">企业服务器。</span><span class="sxs-lookup"><span data-stu-id="55a10-126">Enterprise server.</span></span>|
|<span data-ttu-id="55a10-127">phone</span><span class="sxs-lookup"><span data-stu-id="55a10-127">phone</span></span>|<span data-ttu-id="55a10-128">100</span><span class="sxs-lookup"><span data-stu-id="55a10-128">100</span></span>|<span data-ttu-id="55a10-129">电话。</span><span class="sxs-lookup"><span data-stu-id="55a10-129">Phone.</span></span>|
|<span data-ttu-id="55a10-130">平板电脑</span><span class="sxs-lookup"><span data-stu-id="55a10-130">tablet</span></span>|<span data-ttu-id="55a10-131">101</span><span class="sxs-lookup"><span data-stu-id="55a10-131">101</span></span>|<span data-ttu-id="55a10-132">移动平板电脑。</span><span class="sxs-lookup"><span data-stu-id="55a10-132">Mobile tablet.</span></span>|
|<span data-ttu-id="55a10-133">mobileOther</span><span class="sxs-lookup"><span data-stu-id="55a10-133">mobileOther</span></span>|<span data-ttu-id="55a10-134">102</span><span class="sxs-lookup"><span data-stu-id="55a10-134">102</span></span>|<span data-ttu-id="55a10-135">其他移动。</span><span class="sxs-lookup"><span data-stu-id="55a10-135">Other mobile.</span></span>|
|<span data-ttu-id="55a10-136">mobileUnknown</span><span class="sxs-lookup"><span data-stu-id="55a10-136">mobileUnknown</span></span>|<span data-ttu-id="55a10-137">103</span><span class="sxs-lookup"><span data-stu-id="55a10-137">103</span></span>|<span data-ttu-id="55a10-138">未知移动。</span><span class="sxs-lookup"><span data-stu-id="55a10-138">Unknown mobile.</span></span>|





