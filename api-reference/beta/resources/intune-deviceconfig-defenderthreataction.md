---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563817"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="d87f6-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d87f6-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="d87f6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d87f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d87f6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d87f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d87f6-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="d87f6-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="d87f6-107">成员</span><span class="sxs-lookup"><span data-stu-id="d87f6-107">Members</span></span>
|<span data-ttu-id="d87f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="d87f6-108">Member</span></span>|<span data-ttu-id="d87f6-109">值</span><span class="sxs-lookup"><span data-stu-id="d87f6-109">Value</span></span>|<span data-ttu-id="d87f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="d87f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d87f6-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d87f6-111">deviceDefault</span></span>|<span data-ttu-id="d87f6-112">0</span><span class="sxs-lookup"><span data-stu-id="d87f6-112">0</span></span>|<span data-ttu-id="d87f6-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="d87f6-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="d87f6-114">清理</span><span class="sxs-lookup"><span data-stu-id="d87f6-114">clean</span></span>|<span data-ttu-id="d87f6-115">1</span><span class="sxs-lookup"><span data-stu-id="d87f6-115">1</span></span>|<span data-ttu-id="d87f6-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d87f6-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="d87f6-117">隔离</span><span class="sxs-lookup"><span data-stu-id="d87f6-117">quarantine</span></span>|<span data-ttu-id="d87f6-118">2 </span><span class="sxs-lookup"><span data-stu-id="d87f6-118">2</span></span>|<span data-ttu-id="d87f6-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d87f6-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="d87f6-120">删除</span><span class="sxs-lookup"><span data-stu-id="d87f6-120">remove</span></span>|<span data-ttu-id="d87f6-121">3 </span><span class="sxs-lookup"><span data-stu-id="d87f6-121">3</span></span>|<span data-ttu-id="d87f6-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d87f6-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="d87f6-123">允许</span><span class="sxs-lookup"><span data-stu-id="d87f6-123">allow</span></span>|<span data-ttu-id="d87f6-124">4 </span><span class="sxs-lookup"><span data-stu-id="d87f6-124">4</span></span>|<span data-ttu-id="d87f6-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d87f6-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="d87f6-126">定制</span><span class="sxs-lookup"><span data-stu-id="d87f6-126">userDefined</span></span>|<span data-ttu-id="d87f6-127">5 </span><span class="sxs-lookup"><span data-stu-id="d87f6-127">5</span></span>|<span data-ttu-id="d87f6-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="d87f6-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="d87f6-129">数据</span><span class="sxs-lookup"><span data-stu-id="d87f6-129">block</span></span>|<span data-ttu-id="d87f6-130">6 </span><span class="sxs-lookup"><span data-stu-id="d87f6-130">6</span></span>|<span data-ttu-id="d87f6-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d87f6-131">Block the detected threat.</span></span>|





