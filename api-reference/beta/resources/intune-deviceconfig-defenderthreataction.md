---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4849f369aa5dd04a68599050aa097b2ac63f5ef1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154780"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="3cf2e-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3cf2e-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="3cf2e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cf2e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cf2e-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="3cf2e-107">成员</span><span class="sxs-lookup"><span data-stu-id="3cf2e-107">Members</span></span>
|<span data-ttu-id="3cf2e-108">成员</span><span class="sxs-lookup"><span data-stu-id="3cf2e-108">Member</span></span>|<span data-ttu-id="3cf2e-109">值</span><span class="sxs-lookup"><span data-stu-id="3cf2e-109">Value</span></span>|<span data-ttu-id="3cf2e-110">说明</span><span class="sxs-lookup"><span data-stu-id="3cf2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cf2e-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3cf2e-111">deviceDefault</span></span>|<span data-ttu-id="3cf2e-112">0</span><span class="sxs-lookup"><span data-stu-id="3cf2e-112">0</span></span>|<span data-ttu-id="3cf2e-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="3cf2e-114">clean</span><span class="sxs-lookup"><span data-stu-id="3cf2e-114">clean</span></span>|<span data-ttu-id="3cf2e-115">1</span><span class="sxs-lookup"><span data-stu-id="3cf2e-115">1</span></span>|<span data-ttu-id="3cf2e-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="3cf2e-117">隔离</span><span class="sxs-lookup"><span data-stu-id="3cf2e-117">quarantine</span></span>|<span data-ttu-id="3cf2e-118">双面</span><span class="sxs-lookup"><span data-stu-id="3cf2e-118">2</span></span>|<span data-ttu-id="3cf2e-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="3cf2e-120">删除</span><span class="sxs-lookup"><span data-stu-id="3cf2e-120">remove</span></span>|<span data-ttu-id="3cf2e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3cf2e-121">3</span></span>|<span data-ttu-id="3cf2e-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="3cf2e-123">允许</span><span class="sxs-lookup"><span data-stu-id="3cf2e-123">allow</span></span>|<span data-ttu-id="3cf2e-124">4</span><span class="sxs-lookup"><span data-stu-id="3cf2e-124">4</span></span>|<span data-ttu-id="3cf2e-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="3cf2e-126">定制</span><span class="sxs-lookup"><span data-stu-id="3cf2e-126">userDefined</span></span>|<span data-ttu-id="3cf2e-127">5</span><span class="sxs-lookup"><span data-stu-id="3cf2e-127">5</span></span>|<span data-ttu-id="3cf2e-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="3cf2e-129">数据</span><span class="sxs-lookup"><span data-stu-id="3cf2e-129">block</span></span>|<span data-ttu-id="3cf2e-130">型</span><span class="sxs-lookup"><span data-stu-id="3cf2e-130">6</span></span>|<span data-ttu-id="3cf2e-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="3cf2e-131">Block the detected threat.</span></span>|




