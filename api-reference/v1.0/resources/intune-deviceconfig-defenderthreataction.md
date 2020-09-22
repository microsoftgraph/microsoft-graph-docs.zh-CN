---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d057cf5d052f1fc3043a0b55f4f3ca822f244a7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041454"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="df8ca-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df8ca-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="df8ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df8ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df8ca-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df8ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df8ca-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="df8ca-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="df8ca-107">成员</span><span class="sxs-lookup"><span data-stu-id="df8ca-107">Members</span></span>
|<span data-ttu-id="df8ca-108">成员</span><span class="sxs-lookup"><span data-stu-id="df8ca-108">Member</span></span>|<span data-ttu-id="df8ca-109">值</span><span class="sxs-lookup"><span data-stu-id="df8ca-109">Value</span></span>|<span data-ttu-id="df8ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="df8ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df8ca-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="df8ca-111">deviceDefault</span></span>|<span data-ttu-id="df8ca-112">0</span><span class="sxs-lookup"><span data-stu-id="df8ca-112">0</span></span>|<span data-ttu-id="df8ca-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="df8ca-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="df8ca-114">清理</span><span class="sxs-lookup"><span data-stu-id="df8ca-114">clean</span></span>|<span data-ttu-id="df8ca-115">1 </span><span class="sxs-lookup"><span data-stu-id="df8ca-115">1</span></span>|<span data-ttu-id="df8ca-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="df8ca-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="df8ca-117">隔离</span><span class="sxs-lookup"><span data-stu-id="df8ca-117">quarantine</span></span>|<span data-ttu-id="df8ca-118">2 </span><span class="sxs-lookup"><span data-stu-id="df8ca-118">2</span></span>|<span data-ttu-id="df8ca-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="df8ca-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="df8ca-120">删除</span><span class="sxs-lookup"><span data-stu-id="df8ca-120">remove</span></span>|<span data-ttu-id="df8ca-121">第三章</span><span class="sxs-lookup"><span data-stu-id="df8ca-121">3</span></span>|<span data-ttu-id="df8ca-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="df8ca-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="df8ca-123">允许</span><span class="sxs-lookup"><span data-stu-id="df8ca-123">allow</span></span>|<span data-ttu-id="df8ca-124">4 </span><span class="sxs-lookup"><span data-stu-id="df8ca-124">4</span></span>|<span data-ttu-id="df8ca-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="df8ca-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="df8ca-126">定制</span><span class="sxs-lookup"><span data-stu-id="df8ca-126">userDefined</span></span>|<span data-ttu-id="df8ca-127">5 </span><span class="sxs-lookup"><span data-stu-id="df8ca-127">5</span></span>|<span data-ttu-id="df8ca-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="df8ca-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="df8ca-129">数据</span><span class="sxs-lookup"><span data-stu-id="df8ca-129">block</span></span>|<span data-ttu-id="df8ca-130">6 </span><span class="sxs-lookup"><span data-stu-id="df8ca-130">6</span></span>|<span data-ttu-id="df8ca-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="df8ca-131">Block the detected threat.</span></span>|









