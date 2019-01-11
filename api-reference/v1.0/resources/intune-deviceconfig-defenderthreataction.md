---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
localization_priority: Normal
ms.openlocfilehash: ed84a16dbac493a3e962e37ba246d8d418782a91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852820"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="10048-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="10048-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="10048-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10048-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10048-105">Defender 的默认操作以对其执行检测到恶意软件的威胁。</span><span class="sxs-lookup"><span data-stu-id="10048-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="10048-106">成员</span><span class="sxs-lookup"><span data-stu-id="10048-106">Members</span></span>
|<span data-ttu-id="10048-107">成员</span><span class="sxs-lookup"><span data-stu-id="10048-107">Member</span></span>|<span data-ttu-id="10048-108">值</span><span class="sxs-lookup"><span data-stu-id="10048-108">Value</span></span>|<span data-ttu-id="10048-109">Description</span><span class="sxs-lookup"><span data-stu-id="10048-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10048-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="10048-110">deviceDefault</span></span>|<span data-ttu-id="10048-111">0</span><span class="sxs-lookup"><span data-stu-id="10048-111">0</span></span>|<span data-ttu-id="10048-112">应用基于更新定义的操作。</span><span class="sxs-lookup"><span data-stu-id="10048-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="10048-113">clean</span><span class="sxs-lookup"><span data-stu-id="10048-113">clean</span></span>|<span data-ttu-id="10048-114">1</span><span class="sxs-lookup"><span data-stu-id="10048-114">1</span></span>|<span data-ttu-id="10048-115">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="10048-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="10048-116">隔离</span><span class="sxs-lookup"><span data-stu-id="10048-116">quarantine</span></span>|<span data-ttu-id="10048-117">2</span><span class="sxs-lookup"><span data-stu-id="10048-117">2</span></span>|<span data-ttu-id="10048-118">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="10048-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="10048-119">删除</span><span class="sxs-lookup"><span data-stu-id="10048-119">remove</span></span>|<span data-ttu-id="10048-120">3</span><span class="sxs-lookup"><span data-stu-id="10048-120">3</span></span>|<span data-ttu-id="10048-121">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="10048-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="10048-122">允许</span><span class="sxs-lookup"><span data-stu-id="10048-122">allow</span></span>|<span data-ttu-id="10048-123">4</span><span class="sxs-lookup"><span data-stu-id="10048-123">4</span></span>|<span data-ttu-id="10048-124">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="10048-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="10048-125">用户定制</span><span class="sxs-lookup"><span data-stu-id="10048-125">userDefined</span></span>|<span data-ttu-id="10048-126">5</span><span class="sxs-lookup"><span data-stu-id="10048-126">5</span></span>|<span data-ttu-id="10048-127">允许用户以确定要使用的检测威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="10048-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="10048-128">阻止</span><span class="sxs-lookup"><span data-stu-id="10048-128">block</span></span>|<span data-ttu-id="10048-129">6</span><span class="sxs-lookup"><span data-stu-id="10048-129">6</span></span>|<span data-ttu-id="10048-130">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="10048-130">Block the detected threat.</span></span>|



