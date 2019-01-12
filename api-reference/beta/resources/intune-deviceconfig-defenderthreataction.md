---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: fb54523f2817da328854e57a6672045e46ceb266
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938081"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="b95d2-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b95d2-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="b95d2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b95d2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b95d2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b95d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b95d2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b95d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b95d2-107">Defender 的默认操作以对其执行检测到恶意软件的威胁。</span><span class="sxs-lookup"><span data-stu-id="b95d2-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="b95d2-108">成员</span><span class="sxs-lookup"><span data-stu-id="b95d2-108">Members</span></span>
|<span data-ttu-id="b95d2-109">成员</span><span class="sxs-lookup"><span data-stu-id="b95d2-109">Member</span></span>|<span data-ttu-id="b95d2-110">值</span><span class="sxs-lookup"><span data-stu-id="b95d2-110">Value</span></span>|<span data-ttu-id="b95d2-111">Description</span><span class="sxs-lookup"><span data-stu-id="b95d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b95d2-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b95d2-112">deviceDefault</span></span>|<span data-ttu-id="b95d2-113">0</span><span class="sxs-lookup"><span data-stu-id="b95d2-113">0</span></span>|<span data-ttu-id="b95d2-114">应用基于更新定义的操作。</span><span class="sxs-lookup"><span data-stu-id="b95d2-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="b95d2-115">clean</span><span class="sxs-lookup"><span data-stu-id="b95d2-115">clean</span></span>|<span data-ttu-id="b95d2-116">1</span><span class="sxs-lookup"><span data-stu-id="b95d2-116">1</span></span>|<span data-ttu-id="b95d2-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="b95d2-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="b95d2-118">隔离</span><span class="sxs-lookup"><span data-stu-id="b95d2-118">quarantine</span></span>|<span data-ttu-id="b95d2-119">2</span><span class="sxs-lookup"><span data-stu-id="b95d2-119">2</span></span>|<span data-ttu-id="b95d2-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="b95d2-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="b95d2-121">删除</span><span class="sxs-lookup"><span data-stu-id="b95d2-121">remove</span></span>|<span data-ttu-id="b95d2-122">3</span><span class="sxs-lookup"><span data-stu-id="b95d2-122">3</span></span>|<span data-ttu-id="b95d2-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="b95d2-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="b95d2-124">允许</span><span class="sxs-lookup"><span data-stu-id="b95d2-124">allow</span></span>|<span data-ttu-id="b95d2-125">4</span><span class="sxs-lookup"><span data-stu-id="b95d2-125">4</span></span>|<span data-ttu-id="b95d2-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="b95d2-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="b95d2-127">用户定制</span><span class="sxs-lookup"><span data-stu-id="b95d2-127">userDefined</span></span>|<span data-ttu-id="b95d2-128">5</span><span class="sxs-lookup"><span data-stu-id="b95d2-128">5</span></span>|<span data-ttu-id="b95d2-129">允许用户以确定要使用的检测威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="b95d2-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="b95d2-130">阻止</span><span class="sxs-lookup"><span data-stu-id="b95d2-130">block</span></span>|<span data-ttu-id="b95d2-131">6</span><span class="sxs-lookup"><span data-stu-id="b95d2-131">6</span></span>|<span data-ttu-id="b95d2-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="b95d2-132">Block the detected threat.</span></span>|





