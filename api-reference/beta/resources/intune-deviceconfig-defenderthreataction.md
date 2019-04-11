---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781132"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="00a13-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="00a13-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="00a13-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00a13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00a13-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00a13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00a13-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="00a13-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="00a13-107">成员</span><span class="sxs-lookup"><span data-stu-id="00a13-107">Members</span></span>
|<span data-ttu-id="00a13-108">成员</span><span class="sxs-lookup"><span data-stu-id="00a13-108">Member</span></span>|<span data-ttu-id="00a13-109">值</span><span class="sxs-lookup"><span data-stu-id="00a13-109">Value</span></span>|<span data-ttu-id="00a13-110">说明</span><span class="sxs-lookup"><span data-stu-id="00a13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a13-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="00a13-111">deviceDefault</span></span>|<span data-ttu-id="00a13-112">0</span><span class="sxs-lookup"><span data-stu-id="00a13-112">0</span></span>|<span data-ttu-id="00a13-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="00a13-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="00a13-114">清理</span><span class="sxs-lookup"><span data-stu-id="00a13-114">clean</span></span>|<span data-ttu-id="00a13-115">1</span><span class="sxs-lookup"><span data-stu-id="00a13-115">1</span></span>|<span data-ttu-id="00a13-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="00a13-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="00a13-117">隔离</span><span class="sxs-lookup"><span data-stu-id="00a13-117">quarantine</span></span>|<span data-ttu-id="00a13-118">双面</span><span class="sxs-lookup"><span data-stu-id="00a13-118">2</span></span>|<span data-ttu-id="00a13-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="00a13-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="00a13-120">删除</span><span class="sxs-lookup"><span data-stu-id="00a13-120">remove</span></span>|<span data-ttu-id="00a13-121">第三章</span><span class="sxs-lookup"><span data-stu-id="00a13-121">3</span></span>|<span data-ttu-id="00a13-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="00a13-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="00a13-123">允许</span><span class="sxs-lookup"><span data-stu-id="00a13-123">allow</span></span>|<span data-ttu-id="00a13-124">4</span><span class="sxs-lookup"><span data-stu-id="00a13-124">4</span></span>|<span data-ttu-id="00a13-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="00a13-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="00a13-126">定制</span><span class="sxs-lookup"><span data-stu-id="00a13-126">userDefined</span></span>|<span data-ttu-id="00a13-127">5</span><span class="sxs-lookup"><span data-stu-id="00a13-127">5</span></span>|<span data-ttu-id="00a13-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="00a13-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="00a13-129">数据</span><span class="sxs-lookup"><span data-stu-id="00a13-129">block</span></span>|<span data-ttu-id="00a13-130">型</span><span class="sxs-lookup"><span data-stu-id="00a13-130">6</span></span>|<span data-ttu-id="00a13-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="00a13-131">Block the detected threat.</span></span>|





