---
title: complianceState 枚举类型
description: 合规性状态。
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330273"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="ddfec-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ddfec-103">complianceState enum type</span></span>

> <span data-ttu-id="ddfec-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddfec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddfec-105">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="ddfec-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="ddfec-106">成员</span><span class="sxs-lookup"><span data-stu-id="ddfec-106">Members</span></span>
|<span data-ttu-id="ddfec-107">成员</span><span class="sxs-lookup"><span data-stu-id="ddfec-107">Member</span></span>|<span data-ttu-id="ddfec-108">值</span><span class="sxs-lookup"><span data-stu-id="ddfec-108">Value</span></span>|<span data-ttu-id="ddfec-109">说明</span><span class="sxs-lookup"><span data-stu-id="ddfec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddfec-110">unknown</span><span class="sxs-lookup"><span data-stu-id="ddfec-110">unknown</span></span>|<span data-ttu-id="ddfec-111">0</span><span class="sxs-lookup"><span data-stu-id="ddfec-111">0</span></span>|<span data-ttu-id="ddfec-112">未知。</span><span class="sxs-lookup"><span data-stu-id="ddfec-112">Unknown.</span></span>|
|<span data-ttu-id="ddfec-113">符合标准</span><span class="sxs-lookup"><span data-stu-id="ddfec-113">compliant</span></span>|<span data-ttu-id="ddfec-114">1</span><span class="sxs-lookup"><span data-stu-id="ddfec-114">1</span></span>|<span data-ttu-id="ddfec-115">兼容。</span><span class="sxs-lookup"><span data-stu-id="ddfec-115">Compliant.</span></span>|
|<span data-ttu-id="ddfec-116">不符合标准</span><span class="sxs-lookup"><span data-stu-id="ddfec-116">noncompliant</span></span>|<span data-ttu-id="ddfec-117">2</span><span class="sxs-lookup"><span data-stu-id="ddfec-117">2</span></span>|<span data-ttu-id="ddfec-118">设备不兼容，并阻止从企业资源。</span><span class="sxs-lookup"><span data-stu-id="ddfec-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="ddfec-119">冲突</span><span class="sxs-lookup"><span data-stu-id="ddfec-119">conflict</span></span>|<span data-ttu-id="ddfec-120">3</span><span class="sxs-lookup"><span data-stu-id="ddfec-120">3</span></span>|<span data-ttu-id="ddfec-121">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="ddfec-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="ddfec-122">error</span><span class="sxs-lookup"><span data-stu-id="ddfec-122">error</span></span>|<span data-ttu-id="ddfec-123">4</span><span class="sxs-lookup"><span data-stu-id="ddfec-123">4</span></span>|<span data-ttu-id="ddfec-124">错误。</span><span class="sxs-lookup"><span data-stu-id="ddfec-124">Error.</span></span>|
|<span data-ttu-id="ddfec-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="ddfec-125">inGracePeriod</span></span>|<span data-ttu-id="ddfec-126">254</span><span class="sxs-lookup"><span data-stu-id="ddfec-126">254</span></span>|<span data-ttu-id="ddfec-127">设备不兼容，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="ddfec-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="ddfec-128">configManager</span><span class="sxs-lookup"><span data-stu-id="ddfec-128">configManager</span></span>|<span data-ttu-id="ddfec-129">255</span><span class="sxs-lookup"><span data-stu-id="ddfec-129">255</span></span>|<span data-ttu-id="ddfec-130">配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="ddfec-130">Managed by Config Manager</span></span>|



