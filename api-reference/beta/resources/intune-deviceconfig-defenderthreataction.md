---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
ms.openlocfilehash: d6a4ccbc9725c230f6abc7bd9ee1e38a30d5d133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041489"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="634ec-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="634ec-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="634ec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="634ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="634ec-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="634ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="634ec-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="634ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="634ec-107">Defender 的默认操作以对其执行检测到恶意软件的威胁。</span><span class="sxs-lookup"><span data-stu-id="634ec-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="634ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="634ec-108">Members</span></span>
|<span data-ttu-id="634ec-109">成员</span><span class="sxs-lookup"><span data-stu-id="634ec-109">Member</span></span>|<span data-ttu-id="634ec-110">值</span><span class="sxs-lookup"><span data-stu-id="634ec-110">Value</span></span>|<span data-ttu-id="634ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="634ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="634ec-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="634ec-112">deviceDefault</span></span>|<span data-ttu-id="634ec-113">0</span><span class="sxs-lookup"><span data-stu-id="634ec-113">0</span></span>|<span data-ttu-id="634ec-114">应用基于更新定义的操作。</span><span class="sxs-lookup"><span data-stu-id="634ec-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="634ec-115">clean</span><span class="sxs-lookup"><span data-stu-id="634ec-115">clean</span></span>|<span data-ttu-id="634ec-116">1</span><span class="sxs-lookup"><span data-stu-id="634ec-116">1</span></span>|<span data-ttu-id="634ec-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="634ec-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="634ec-118">隔离</span><span class="sxs-lookup"><span data-stu-id="634ec-118">quarantine</span></span>|<span data-ttu-id="634ec-119">2</span><span class="sxs-lookup"><span data-stu-id="634ec-119">2</span></span>|<span data-ttu-id="634ec-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="634ec-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="634ec-121">删除</span><span class="sxs-lookup"><span data-stu-id="634ec-121">remove</span></span>|<span data-ttu-id="634ec-122">3</span><span class="sxs-lookup"><span data-stu-id="634ec-122">3</span></span>|<span data-ttu-id="634ec-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="634ec-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="634ec-124">允许</span><span class="sxs-lookup"><span data-stu-id="634ec-124">allow</span></span>|<span data-ttu-id="634ec-125">4</span><span class="sxs-lookup"><span data-stu-id="634ec-125">4</span></span>|<span data-ttu-id="634ec-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="634ec-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="634ec-127">用户定制</span><span class="sxs-lookup"><span data-stu-id="634ec-127">userDefined</span></span>|<span data-ttu-id="634ec-128">5</span><span class="sxs-lookup"><span data-stu-id="634ec-128">5</span></span>|<span data-ttu-id="634ec-129">允许用户以确定要使用的检测威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="634ec-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="634ec-130">阻止</span><span class="sxs-lookup"><span data-stu-id="634ec-130">block</span></span>|<span data-ttu-id="634ec-131">6</span><span class="sxs-lookup"><span data-stu-id="634ec-131">6</span></span>|<span data-ttu-id="634ec-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="634ec-132">Block the detected threat.</span></span>|





