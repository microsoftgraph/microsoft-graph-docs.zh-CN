---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6549b16e325fd8830d0b96de7fd234a315319b8a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794408"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="d3f6b-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3f6b-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="d3f6b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3f6b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3f6b-106">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="d3f6b-107">成员</span><span class="sxs-lookup"><span data-stu-id="d3f6b-107">Members</span></span>
|<span data-ttu-id="d3f6b-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3f6b-108">Member</span></span>|<span data-ttu-id="d3f6b-109">值</span><span class="sxs-lookup"><span data-stu-id="d3f6b-109">Value</span></span>|<span data-ttu-id="d3f6b-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3f6b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f6b-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d3f6b-111">deviceDefault</span></span>|<span data-ttu-id="d3f6b-112">0</span><span class="sxs-lookup"><span data-stu-id="d3f6b-112">0</span></span>|<span data-ttu-id="d3f6b-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="d3f6b-114">清理</span><span class="sxs-lookup"><span data-stu-id="d3f6b-114">clean</span></span>|<span data-ttu-id="d3f6b-115">1</span><span class="sxs-lookup"><span data-stu-id="d3f6b-115">1</span></span>|<span data-ttu-id="d3f6b-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="d3f6b-117">隔离</span><span class="sxs-lookup"><span data-stu-id="d3f6b-117">quarantine</span></span>|<span data-ttu-id="d3f6b-118">双面</span><span class="sxs-lookup"><span data-stu-id="d3f6b-118">2</span></span>|<span data-ttu-id="d3f6b-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="d3f6b-120">删除</span><span class="sxs-lookup"><span data-stu-id="d3f6b-120">remove</span></span>|<span data-ttu-id="d3f6b-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d3f6b-121">3</span></span>|<span data-ttu-id="d3f6b-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="d3f6b-123">允许</span><span class="sxs-lookup"><span data-stu-id="d3f6b-123">allow</span></span>|<span data-ttu-id="d3f6b-124">4 </span><span class="sxs-lookup"><span data-stu-id="d3f6b-124">4</span></span>|<span data-ttu-id="d3f6b-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="d3f6b-126">定制</span><span class="sxs-lookup"><span data-stu-id="d3f6b-126">userDefined</span></span>|<span data-ttu-id="d3f6b-127">5 </span><span class="sxs-lookup"><span data-stu-id="d3f6b-127">5</span></span>|<span data-ttu-id="d3f6b-128">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="d3f6b-129">数据</span><span class="sxs-lookup"><span data-stu-id="d3f6b-129">block</span></span>|<span data-ttu-id="d3f6b-130">6 </span><span class="sxs-lookup"><span data-stu-id="d3f6b-130">6</span></span>|<span data-ttu-id="d3f6b-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d3f6b-131">Block the detected threat.</span></span>|



