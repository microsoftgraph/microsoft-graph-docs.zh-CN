---
title: complianceState 枚举类型
description: 合规性状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392736"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="498a1-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="498a1-103">complianceState enum type</span></span>

> <span data-ttu-id="498a1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="498a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="498a1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="498a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="498a1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="498a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="498a1-107">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="498a1-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="498a1-108">成员</span><span class="sxs-lookup"><span data-stu-id="498a1-108">Members</span></span>
|<span data-ttu-id="498a1-109">成员</span><span class="sxs-lookup"><span data-stu-id="498a1-109">Member</span></span>|<span data-ttu-id="498a1-110">值</span><span class="sxs-lookup"><span data-stu-id="498a1-110">Value</span></span>|<span data-ttu-id="498a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="498a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="498a1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="498a1-112">unknown</span></span>|<span data-ttu-id="498a1-113">0</span><span class="sxs-lookup"><span data-stu-id="498a1-113">0</span></span>|<span data-ttu-id="498a1-114">未知。</span><span class="sxs-lookup"><span data-stu-id="498a1-114">Unknown.</span></span>|
|<span data-ttu-id="498a1-115">符合标准</span><span class="sxs-lookup"><span data-stu-id="498a1-115">compliant</span></span>|<span data-ttu-id="498a1-116">1</span><span class="sxs-lookup"><span data-stu-id="498a1-116">1</span></span>|<span data-ttu-id="498a1-117">兼容。</span><span class="sxs-lookup"><span data-stu-id="498a1-117">Compliant.</span></span>|
|<span data-ttu-id="498a1-118">不符合标准</span><span class="sxs-lookup"><span data-stu-id="498a1-118">noncompliant</span></span>|<span data-ttu-id="498a1-119">2</span><span class="sxs-lookup"><span data-stu-id="498a1-119">2</span></span>|<span data-ttu-id="498a1-120">设备不兼容，并阻止从企业资源。</span><span class="sxs-lookup"><span data-stu-id="498a1-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="498a1-121">冲突</span><span class="sxs-lookup"><span data-stu-id="498a1-121">conflict</span></span>|<span data-ttu-id="498a1-122">3</span><span class="sxs-lookup"><span data-stu-id="498a1-122">3</span></span>|<span data-ttu-id="498a1-123">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="498a1-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="498a1-124">error</span><span class="sxs-lookup"><span data-stu-id="498a1-124">error</span></span>|<span data-ttu-id="498a1-125">4</span><span class="sxs-lookup"><span data-stu-id="498a1-125">4</span></span>|<span data-ttu-id="498a1-126">错误。</span><span class="sxs-lookup"><span data-stu-id="498a1-126">Error.</span></span>|
|<span data-ttu-id="498a1-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="498a1-127">inGracePeriod</span></span>|<span data-ttu-id="498a1-128">254</span><span class="sxs-lookup"><span data-stu-id="498a1-128">254</span></span>|<span data-ttu-id="498a1-129">设备不兼容，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="498a1-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="498a1-130">configManager</span><span class="sxs-lookup"><span data-stu-id="498a1-130">configManager</span></span>|<span data-ttu-id="498a1-131">255</span><span class="sxs-lookup"><span data-stu-id="498a1-131">255</span></span>|<span data-ttu-id="498a1-132">配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="498a1-132">Managed by Config Manager</span></span>|




