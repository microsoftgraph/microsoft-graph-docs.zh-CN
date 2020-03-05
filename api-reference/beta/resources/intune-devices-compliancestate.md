---
title: complianceState 枚举类型
description: 合规性状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78dc7dfee02a1b1670a2259d20465d4660e73a08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525150"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="06565-103">complianceState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="06565-103">complianceState enum type</span></span>

<span data-ttu-id="06565-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="06565-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06565-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06565-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06565-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06565-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06565-107">合规性状态。</span><span class="sxs-lookup"><span data-stu-id="06565-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="06565-108">成员</span><span class="sxs-lookup"><span data-stu-id="06565-108">Members</span></span>
|<span data-ttu-id="06565-109">成员</span><span class="sxs-lookup"><span data-stu-id="06565-109">Member</span></span>|<span data-ttu-id="06565-110">值</span><span class="sxs-lookup"><span data-stu-id="06565-110">Value</span></span>|<span data-ttu-id="06565-111">说明</span><span class="sxs-lookup"><span data-stu-id="06565-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06565-112">unknown</span><span class="sxs-lookup"><span data-stu-id="06565-112">unknown</span></span>|<span data-ttu-id="06565-113">0</span><span class="sxs-lookup"><span data-stu-id="06565-113">0</span></span>|<span data-ttu-id="06565-114">陌生.</span><span class="sxs-lookup"><span data-stu-id="06565-114">Unknown.</span></span>|
|<span data-ttu-id="06565-115">合格</span><span class="sxs-lookup"><span data-stu-id="06565-115">compliant</span></span>|<span data-ttu-id="06565-116">1 </span><span class="sxs-lookup"><span data-stu-id="06565-116">1</span></span>|<span data-ttu-id="06565-117">合格.</span><span class="sxs-lookup"><span data-stu-id="06565-117">Compliant.</span></span>|
|<span data-ttu-id="06565-118">合规</span><span class="sxs-lookup"><span data-stu-id="06565-118">noncompliant</span></span>|<span data-ttu-id="06565-119">2 </span><span class="sxs-lookup"><span data-stu-id="06565-119">2</span></span>|<span data-ttu-id="06565-120">设备不合规，并将从公司资源中阻止。</span><span class="sxs-lookup"><span data-stu-id="06565-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="06565-121">冲突</span><span class="sxs-lookup"><span data-stu-id="06565-121">conflict</span></span>|<span data-ttu-id="06565-122">3 </span><span class="sxs-lookup"><span data-stu-id="06565-122">3</span></span>|<span data-ttu-id="06565-123">与其他规则冲突。</span><span class="sxs-lookup"><span data-stu-id="06565-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="06565-124">error</span><span class="sxs-lookup"><span data-stu-id="06565-124">error</span></span>|<span data-ttu-id="06565-125">4 </span><span class="sxs-lookup"><span data-stu-id="06565-125">4</span></span>|<span data-ttu-id="06565-126">错误。</span><span class="sxs-lookup"><span data-stu-id="06565-126">Error.</span></span>|
|<span data-ttu-id="06565-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="06565-127">inGracePeriod</span></span>|<span data-ttu-id="06565-128">254</span><span class="sxs-lookup"><span data-stu-id="06565-128">254</span></span>|<span data-ttu-id="06565-129">Device 不合规，但仍有权访问公司资源</span><span class="sxs-lookup"><span data-stu-id="06565-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="06565-130">configManager</span><span class="sxs-lookup"><span data-stu-id="06565-130">configManager</span></span>|<span data-ttu-id="06565-131">255</span><span class="sxs-lookup"><span data-stu-id="06565-131">255</span></span>|<span data-ttu-id="06565-132">由配置管理器管理</span><span class="sxs-lookup"><span data-stu-id="06565-132">Managed by Config Manager</span></span>|



