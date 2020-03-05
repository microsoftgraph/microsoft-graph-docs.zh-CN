---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fda734d6d582f8b838e0dca26ae57c118f3438b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526833"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="40579-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="40579-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="40579-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="40579-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40579-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40579-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40579-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40579-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40579-107">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="40579-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="40579-108">成员</span><span class="sxs-lookup"><span data-stu-id="40579-108">Members</span></span>
|<span data-ttu-id="40579-109">成员</span><span class="sxs-lookup"><span data-stu-id="40579-109">Member</span></span>|<span data-ttu-id="40579-110">值</span><span class="sxs-lookup"><span data-stu-id="40579-110">Value</span></span>|<span data-ttu-id="40579-111">说明</span><span class="sxs-lookup"><span data-stu-id="40579-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40579-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="40579-112">deviceDefault</span></span>|<span data-ttu-id="40579-113">0</span><span class="sxs-lookup"><span data-stu-id="40579-113">0</span></span>|<span data-ttu-id="40579-114">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="40579-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="40579-115">清理</span><span class="sxs-lookup"><span data-stu-id="40579-115">clean</span></span>|<span data-ttu-id="40579-116">1 </span><span class="sxs-lookup"><span data-stu-id="40579-116">1</span></span>|<span data-ttu-id="40579-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="40579-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="40579-118">隔离</span><span class="sxs-lookup"><span data-stu-id="40579-118">quarantine</span></span>|<span data-ttu-id="40579-119">2 </span><span class="sxs-lookup"><span data-stu-id="40579-119">2</span></span>|<span data-ttu-id="40579-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="40579-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="40579-121">删除</span><span class="sxs-lookup"><span data-stu-id="40579-121">remove</span></span>|<span data-ttu-id="40579-122">3 </span><span class="sxs-lookup"><span data-stu-id="40579-122">3</span></span>|<span data-ttu-id="40579-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="40579-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="40579-124">允许</span><span class="sxs-lookup"><span data-stu-id="40579-124">allow</span></span>|<span data-ttu-id="40579-125">4 </span><span class="sxs-lookup"><span data-stu-id="40579-125">4</span></span>|<span data-ttu-id="40579-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="40579-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="40579-127">定制</span><span class="sxs-lookup"><span data-stu-id="40579-127">userDefined</span></span>|<span data-ttu-id="40579-128">5 </span><span class="sxs-lookup"><span data-stu-id="40579-128">5</span></span>|<span data-ttu-id="40579-129">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="40579-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="40579-130">数据</span><span class="sxs-lookup"><span data-stu-id="40579-130">block</span></span>|<span data-ttu-id="40579-131">6 </span><span class="sxs-lookup"><span data-stu-id="40579-131">6</span></span>|<span data-ttu-id="40579-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="40579-132">Block the detected threat.</span></span>|



