---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24c2b0c60f0451b58e624558fd44f3628c92e3cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448986"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="5caf1-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5caf1-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="5caf1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5caf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5caf1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5caf1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5caf1-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="5caf1-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="5caf1-107">成员</span><span class="sxs-lookup"><span data-stu-id="5caf1-107">Members</span></span>
|<span data-ttu-id="5caf1-108">成员</span><span class="sxs-lookup"><span data-stu-id="5caf1-108">Member</span></span>|<span data-ttu-id="5caf1-109">值</span><span class="sxs-lookup"><span data-stu-id="5caf1-109">Value</span></span>|<span data-ttu-id="5caf1-110">说明</span><span class="sxs-lookup"><span data-stu-id="5caf1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5caf1-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5caf1-111">deviceDefault</span></span>|<span data-ttu-id="5caf1-112">0</span><span class="sxs-lookup"><span data-stu-id="5caf1-112">0</span></span>|<span data-ttu-id="5caf1-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="5caf1-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="5caf1-114">清理</span><span class="sxs-lookup"><span data-stu-id="5caf1-114">clean</span></span>|<span data-ttu-id="5caf1-115">1</span><span class="sxs-lookup"><span data-stu-id="5caf1-115">1</span></span>|<span data-ttu-id="5caf1-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="5caf1-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="5caf1-117">隔离</span><span class="sxs-lookup"><span data-stu-id="5caf1-117">quarantine</span></span>|<span data-ttu-id="5caf1-118">双面</span><span class="sxs-lookup"><span data-stu-id="5caf1-118">2</span></span>|<span data-ttu-id="5caf1-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="5caf1-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="5caf1-120">删除</span><span class="sxs-lookup"><span data-stu-id="5caf1-120">remove</span></span>|<span data-ttu-id="5caf1-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5caf1-121">3</span></span>|<span data-ttu-id="5caf1-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="5caf1-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="5caf1-123">允许</span><span class="sxs-lookup"><span data-stu-id="5caf1-123">allow</span></span>|<span data-ttu-id="5caf1-124">4 </span><span class="sxs-lookup"><span data-stu-id="5caf1-124">4</span></span>|<span data-ttu-id="5caf1-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="5caf1-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="5caf1-126">定制</span><span class="sxs-lookup"><span data-stu-id="5caf1-126">userDefined</span></span>|<span data-ttu-id="5caf1-127">5 </span><span class="sxs-lookup"><span data-stu-id="5caf1-127">5</span></span>|<span data-ttu-id="5caf1-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="5caf1-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="5caf1-129">数据</span><span class="sxs-lookup"><span data-stu-id="5caf1-129">block</span></span>|<span data-ttu-id="5caf1-130">6 </span><span class="sxs-lookup"><span data-stu-id="5caf1-130">6</span></span>|<span data-ttu-id="5caf1-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="5caf1-131">Block the detected threat.</span></span>|







