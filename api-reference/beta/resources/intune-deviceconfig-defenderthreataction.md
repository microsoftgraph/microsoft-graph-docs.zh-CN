---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd72afa1d49e39486454304ce27517e9433a137a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420799"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="45d46-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="45d46-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="45d46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45d46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45d46-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="45d46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d46-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45d46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d46-107">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="45d46-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="45d46-108">成员</span><span class="sxs-lookup"><span data-stu-id="45d46-108">Members</span></span>
|<span data-ttu-id="45d46-109">成员</span><span class="sxs-lookup"><span data-stu-id="45d46-109">Member</span></span>|<span data-ttu-id="45d46-110">值</span><span class="sxs-lookup"><span data-stu-id="45d46-110">Value</span></span>|<span data-ttu-id="45d46-111">说明</span><span class="sxs-lookup"><span data-stu-id="45d46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d46-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="45d46-112">deviceDefault</span></span>|<span data-ttu-id="45d46-113">0</span><span class="sxs-lookup"><span data-stu-id="45d46-113">0</span></span>|<span data-ttu-id="45d46-114">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="45d46-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="45d46-115">清理</span><span class="sxs-lookup"><span data-stu-id="45d46-115">clean</span></span>|<span data-ttu-id="45d46-116">1</span><span class="sxs-lookup"><span data-stu-id="45d46-116">1</span></span>|<span data-ttu-id="45d46-117">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45d46-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="45d46-118">隔离</span><span class="sxs-lookup"><span data-stu-id="45d46-118">quarantine</span></span>|<span data-ttu-id="45d46-119">双面</span><span class="sxs-lookup"><span data-stu-id="45d46-119">2</span></span>|<span data-ttu-id="45d46-120">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45d46-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="45d46-121">删除</span><span class="sxs-lookup"><span data-stu-id="45d46-121">remove</span></span>|<span data-ttu-id="45d46-122">第三章</span><span class="sxs-lookup"><span data-stu-id="45d46-122">3</span></span>|<span data-ttu-id="45d46-123">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45d46-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="45d46-124">允许</span><span class="sxs-lookup"><span data-stu-id="45d46-124">allow</span></span>|<span data-ttu-id="45d46-125">4 </span><span class="sxs-lookup"><span data-stu-id="45d46-125">4</span></span>|<span data-ttu-id="45d46-126">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45d46-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="45d46-127">定制</span><span class="sxs-lookup"><span data-stu-id="45d46-127">userDefined</span></span>|<span data-ttu-id="45d46-128">5 </span><span class="sxs-lookup"><span data-stu-id="45d46-128">5</span></span>|<span data-ttu-id="45d46-129">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="45d46-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="45d46-130">数据</span><span class="sxs-lookup"><span data-stu-id="45d46-130">block</span></span>|<span data-ttu-id="45d46-131">6 </span><span class="sxs-lookup"><span data-stu-id="45d46-131">6</span></span>|<span data-ttu-id="45d46-132">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="45d46-132">Block the detected threat.</span></span>|



