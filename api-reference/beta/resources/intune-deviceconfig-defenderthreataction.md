---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d93ed616a73c69467a1a77cb27e6fb27a7ea553
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024295"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="3d9ea-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3d9ea-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="3d9ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d9ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d9ea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d9ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d9ea-107">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="3d9ea-108">成员</span><span class="sxs-lookup"><span data-stu-id="3d9ea-108">Members</span></span>
|<span data-ttu-id="3d9ea-109">成员</span><span class="sxs-lookup"><span data-stu-id="3d9ea-109">Member</span></span>|<span data-ttu-id="3d9ea-110">值</span><span class="sxs-lookup"><span data-stu-id="3d9ea-110">Value</span></span>|<span data-ttu-id="3d9ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d9ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d9ea-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3d9ea-112">deviceDefault</span></span>|<span data-ttu-id="3d9ea-113">0</span><span class="sxs-lookup"><span data-stu-id="3d9ea-113">0</span></span>|<span data-ttu-id="3d9ea-114">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="3d9ea-115">清理</span><span class="sxs-lookup"><span data-stu-id="3d9ea-115">clean</span></span>|<span data-ttu-id="3d9ea-116">1 </span><span class="sxs-lookup"><span data-stu-id="3d9ea-116">1</span></span>|<span data-ttu-id="3d9ea-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="3d9ea-118">隔离</span><span class="sxs-lookup"><span data-stu-id="3d9ea-118">quarantine</span></span>|<span data-ttu-id="3d9ea-119">2 </span><span class="sxs-lookup"><span data-stu-id="3d9ea-119">2</span></span>|<span data-ttu-id="3d9ea-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="3d9ea-121">删除</span><span class="sxs-lookup"><span data-stu-id="3d9ea-121">remove</span></span>|<span data-ttu-id="3d9ea-122">第三章</span><span class="sxs-lookup"><span data-stu-id="3d9ea-122">3</span></span>|<span data-ttu-id="3d9ea-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="3d9ea-124">允许</span><span class="sxs-lookup"><span data-stu-id="3d9ea-124">allow</span></span>|<span data-ttu-id="3d9ea-125">4 </span><span class="sxs-lookup"><span data-stu-id="3d9ea-125">4</span></span>|<span data-ttu-id="3d9ea-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="3d9ea-127">定制</span><span class="sxs-lookup"><span data-stu-id="3d9ea-127">userDefined</span></span>|<span data-ttu-id="3d9ea-128">5 </span><span class="sxs-lookup"><span data-stu-id="3d9ea-128">5</span></span>|<span data-ttu-id="3d9ea-129">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="3d9ea-130">数据</span><span class="sxs-lookup"><span data-stu-id="3d9ea-130">block</span></span>|<span data-ttu-id="3d9ea-131">6 </span><span class="sxs-lookup"><span data-stu-id="3d9ea-131">6</span></span>|<span data-ttu-id="3d9ea-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3d9ea-132">Block the detected threat.</span></span>|






