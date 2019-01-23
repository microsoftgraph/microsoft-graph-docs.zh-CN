---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400268"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="45611-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="45611-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="45611-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="45611-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45611-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45611-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45611-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45611-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45611-107">Defender 的默认操作以对其执行检测到恶意软件的威胁。</span><span class="sxs-lookup"><span data-stu-id="45611-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="45611-108">成员</span><span class="sxs-lookup"><span data-stu-id="45611-108">Members</span></span>
|<span data-ttu-id="45611-109">成员</span><span class="sxs-lookup"><span data-stu-id="45611-109">Member</span></span>|<span data-ttu-id="45611-110">值</span><span class="sxs-lookup"><span data-stu-id="45611-110">Value</span></span>|<span data-ttu-id="45611-111">说明</span><span class="sxs-lookup"><span data-stu-id="45611-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45611-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="45611-112">deviceDefault</span></span>|<span data-ttu-id="45611-113">0</span><span class="sxs-lookup"><span data-stu-id="45611-113">0</span></span>|<span data-ttu-id="45611-114">应用基于更新定义的操作。</span><span class="sxs-lookup"><span data-stu-id="45611-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="45611-115">clean</span><span class="sxs-lookup"><span data-stu-id="45611-115">clean</span></span>|<span data-ttu-id="45611-116">1</span><span class="sxs-lookup"><span data-stu-id="45611-116">1</span></span>|<span data-ttu-id="45611-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45611-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="45611-118">隔离</span><span class="sxs-lookup"><span data-stu-id="45611-118">quarantine</span></span>|<span data-ttu-id="45611-119">2</span><span class="sxs-lookup"><span data-stu-id="45611-119">2</span></span>|<span data-ttu-id="45611-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45611-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="45611-121">删除</span><span class="sxs-lookup"><span data-stu-id="45611-121">remove</span></span>|<span data-ttu-id="45611-122">3</span><span class="sxs-lookup"><span data-stu-id="45611-122">3</span></span>|<span data-ttu-id="45611-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45611-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="45611-124">允许</span><span class="sxs-lookup"><span data-stu-id="45611-124">allow</span></span>|<span data-ttu-id="45611-125">4</span><span class="sxs-lookup"><span data-stu-id="45611-125">4</span></span>|<span data-ttu-id="45611-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45611-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="45611-127">用户定制</span><span class="sxs-lookup"><span data-stu-id="45611-127">userDefined</span></span>|<span data-ttu-id="45611-128">5</span><span class="sxs-lookup"><span data-stu-id="45611-128">5</span></span>|<span data-ttu-id="45611-129">允许用户以确定要使用的检测威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="45611-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="45611-130">阻止</span><span class="sxs-lookup"><span data-stu-id="45611-130">block</span></span>|<span data-ttu-id="45611-131">6</span><span class="sxs-lookup"><span data-stu-id="45611-131">6</span></span>|<span data-ttu-id="45611-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45611-132">Block the detected threat.</span></span>|




