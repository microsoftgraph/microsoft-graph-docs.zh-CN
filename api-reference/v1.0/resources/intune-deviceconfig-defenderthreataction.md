---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 71533fa6d01c9c51980881429b4dc3e443f9c766
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359675"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="86f97-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="86f97-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="86f97-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86f97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86f97-105">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="86f97-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="86f97-106">成员</span><span class="sxs-lookup"><span data-stu-id="86f97-106">Members</span></span>
|<span data-ttu-id="86f97-107">成员</span><span class="sxs-lookup"><span data-stu-id="86f97-107">Member</span></span>|<span data-ttu-id="86f97-108">值</span><span class="sxs-lookup"><span data-stu-id="86f97-108">Value</span></span>|<span data-ttu-id="86f97-109">说明</span><span class="sxs-lookup"><span data-stu-id="86f97-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86f97-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="86f97-110">deviceDefault</span></span>|<span data-ttu-id="86f97-111">0</span><span class="sxs-lookup"><span data-stu-id="86f97-111">0</span></span>|<span data-ttu-id="86f97-112">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="86f97-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="86f97-113">清理</span><span class="sxs-lookup"><span data-stu-id="86f97-113">clean</span></span>|<span data-ttu-id="86f97-114">1</span><span class="sxs-lookup"><span data-stu-id="86f97-114">1</span></span>|<span data-ttu-id="86f97-115">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="86f97-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="86f97-116">隔离</span><span class="sxs-lookup"><span data-stu-id="86f97-116">quarantine</span></span>|<span data-ttu-id="86f97-117">双面</span><span class="sxs-lookup"><span data-stu-id="86f97-117">2</span></span>|<span data-ttu-id="86f97-118">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="86f97-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="86f97-119">删除</span><span class="sxs-lookup"><span data-stu-id="86f97-119">remove</span></span>|<span data-ttu-id="86f97-120">第三章</span><span class="sxs-lookup"><span data-stu-id="86f97-120">3</span></span>|<span data-ttu-id="86f97-121">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="86f97-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="86f97-122">允许</span><span class="sxs-lookup"><span data-stu-id="86f97-122">allow</span></span>|<span data-ttu-id="86f97-123">4</span><span class="sxs-lookup"><span data-stu-id="86f97-123">4</span></span>|<span data-ttu-id="86f97-124">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="86f97-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="86f97-125">定制</span><span class="sxs-lookup"><span data-stu-id="86f97-125">userDefined</span></span>|<span data-ttu-id="86f97-126">5</span><span class="sxs-lookup"><span data-stu-id="86f97-126">5</span></span>|<span data-ttu-id="86f97-127">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="86f97-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="86f97-128">数据</span><span class="sxs-lookup"><span data-stu-id="86f97-128">block</span></span>|<span data-ttu-id="86f97-129">型</span><span class="sxs-lookup"><span data-stu-id="86f97-129">6</span></span>|<span data-ttu-id="86f97-130">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="86f97-130">Block the detected threat.</span></span>|




