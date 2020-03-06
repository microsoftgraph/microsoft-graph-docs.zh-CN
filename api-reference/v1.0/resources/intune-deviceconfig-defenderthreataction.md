---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4c9edcd596d6dcd40b2cfe873b660651f74bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530856"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="eb37d-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="eb37d-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="eb37d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb37d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb37d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb37d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb37d-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="eb37d-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="eb37d-107">成员</span><span class="sxs-lookup"><span data-stu-id="eb37d-107">Members</span></span>
|<span data-ttu-id="eb37d-108">成员</span><span class="sxs-lookup"><span data-stu-id="eb37d-108">Member</span></span>|<span data-ttu-id="eb37d-109">值</span><span class="sxs-lookup"><span data-stu-id="eb37d-109">Value</span></span>|<span data-ttu-id="eb37d-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb37d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb37d-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="eb37d-111">deviceDefault</span></span>|<span data-ttu-id="eb37d-112">0</span><span class="sxs-lookup"><span data-stu-id="eb37d-112">0</span></span>|<span data-ttu-id="eb37d-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="eb37d-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="eb37d-114">清理</span><span class="sxs-lookup"><span data-stu-id="eb37d-114">clean</span></span>|<span data-ttu-id="eb37d-115">1 </span><span class="sxs-lookup"><span data-stu-id="eb37d-115">1</span></span>|<span data-ttu-id="eb37d-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="eb37d-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="eb37d-117">隔离</span><span class="sxs-lookup"><span data-stu-id="eb37d-117">quarantine</span></span>|<span data-ttu-id="eb37d-118">2 </span><span class="sxs-lookup"><span data-stu-id="eb37d-118">2</span></span>|<span data-ttu-id="eb37d-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="eb37d-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="eb37d-120">删除</span><span class="sxs-lookup"><span data-stu-id="eb37d-120">remove</span></span>|<span data-ttu-id="eb37d-121">3 </span><span class="sxs-lookup"><span data-stu-id="eb37d-121">3</span></span>|<span data-ttu-id="eb37d-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="eb37d-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="eb37d-123">允许</span><span class="sxs-lookup"><span data-stu-id="eb37d-123">allow</span></span>|<span data-ttu-id="eb37d-124">4 </span><span class="sxs-lookup"><span data-stu-id="eb37d-124">4</span></span>|<span data-ttu-id="eb37d-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="eb37d-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="eb37d-126">定制</span><span class="sxs-lookup"><span data-stu-id="eb37d-126">userDefined</span></span>|<span data-ttu-id="eb37d-127">5 </span><span class="sxs-lookup"><span data-stu-id="eb37d-127">5</span></span>|<span data-ttu-id="eb37d-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="eb37d-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="eb37d-129">数据</span><span class="sxs-lookup"><span data-stu-id="eb37d-129">block</span></span>|<span data-ttu-id="eb37d-130">6 </span><span class="sxs-lookup"><span data-stu-id="eb37d-130">6</span></span>|<span data-ttu-id="eb37d-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="eb37d-131">Block the detected threat.</span></span>|




