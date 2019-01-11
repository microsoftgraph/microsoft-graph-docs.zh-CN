---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
localization_priority: Normal
ms.openlocfilehash: 7e448e6fae0ebbb0f14a3b7932e6f306a70588b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837868"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="ab244-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab244-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="ab244-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab244-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab244-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab244-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab244-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ab244-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab244-107">Defender 的默认操作以对其执行检测到恶意软件的威胁。</span><span class="sxs-lookup"><span data-stu-id="ab244-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="ab244-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab244-108">Members</span></span>
|<span data-ttu-id="ab244-109">成员</span><span class="sxs-lookup"><span data-stu-id="ab244-109">Member</span></span>|<span data-ttu-id="ab244-110">值</span><span class="sxs-lookup"><span data-stu-id="ab244-110">Value</span></span>|<span data-ttu-id="ab244-111">Description</span><span class="sxs-lookup"><span data-stu-id="ab244-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab244-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ab244-112">deviceDefault</span></span>|<span data-ttu-id="ab244-113">0</span><span class="sxs-lookup"><span data-stu-id="ab244-113">0</span></span>|<span data-ttu-id="ab244-114">应用基于更新定义的操作。</span><span class="sxs-lookup"><span data-stu-id="ab244-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="ab244-115">clean</span><span class="sxs-lookup"><span data-stu-id="ab244-115">clean</span></span>|<span data-ttu-id="ab244-116">1</span><span class="sxs-lookup"><span data-stu-id="ab244-116">1</span></span>|<span data-ttu-id="ab244-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="ab244-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="ab244-118">隔离</span><span class="sxs-lookup"><span data-stu-id="ab244-118">quarantine</span></span>|<span data-ttu-id="ab244-119">2</span><span class="sxs-lookup"><span data-stu-id="ab244-119">2</span></span>|<span data-ttu-id="ab244-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="ab244-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="ab244-121">删除</span><span class="sxs-lookup"><span data-stu-id="ab244-121">remove</span></span>|<span data-ttu-id="ab244-122">3</span><span class="sxs-lookup"><span data-stu-id="ab244-122">3</span></span>|<span data-ttu-id="ab244-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="ab244-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="ab244-124">允许</span><span class="sxs-lookup"><span data-stu-id="ab244-124">allow</span></span>|<span data-ttu-id="ab244-125">4</span><span class="sxs-lookup"><span data-stu-id="ab244-125">4</span></span>|<span data-ttu-id="ab244-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="ab244-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="ab244-127">用户定制</span><span class="sxs-lookup"><span data-stu-id="ab244-127">userDefined</span></span>|<span data-ttu-id="ab244-128">5</span><span class="sxs-lookup"><span data-stu-id="ab244-128">5</span></span>|<span data-ttu-id="ab244-129">允许用户以确定要使用的检测威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="ab244-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="ab244-130">阻止</span><span class="sxs-lookup"><span data-stu-id="ab244-130">block</span></span>|<span data-ttu-id="ab244-131">6</span><span class="sxs-lookup"><span data-stu-id="ab244-131">6</span></span>|<span data-ttu-id="ab244-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="ab244-132">Block the detected threat.</span></span>|





