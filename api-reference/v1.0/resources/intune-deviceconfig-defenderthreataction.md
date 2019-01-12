---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976644"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="2f9d3-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2f9d3-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="2f9d3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f9d3-105">Defender 的默认操作以对其执行检测到恶意软件的威胁。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="2f9d3-106">成员</span><span class="sxs-lookup"><span data-stu-id="2f9d3-106">Members</span></span>
|<span data-ttu-id="2f9d3-107">成员</span><span class="sxs-lookup"><span data-stu-id="2f9d3-107">Member</span></span>|<span data-ttu-id="2f9d3-108">值</span><span class="sxs-lookup"><span data-stu-id="2f9d3-108">Value</span></span>|<span data-ttu-id="2f9d3-109">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9d3-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2f9d3-110">deviceDefault</span></span>|<span data-ttu-id="2f9d3-111">0</span><span class="sxs-lookup"><span data-stu-id="2f9d3-111">0</span></span>|<span data-ttu-id="2f9d3-112">应用基于更新定义的操作。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="2f9d3-113">clean</span><span class="sxs-lookup"><span data-stu-id="2f9d3-113">clean</span></span>|<span data-ttu-id="2f9d3-114">1</span><span class="sxs-lookup"><span data-stu-id="2f9d3-114">1</span></span>|<span data-ttu-id="2f9d3-115">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="2f9d3-116">隔离</span><span class="sxs-lookup"><span data-stu-id="2f9d3-116">quarantine</span></span>|<span data-ttu-id="2f9d3-117">2</span><span class="sxs-lookup"><span data-stu-id="2f9d3-117">2</span></span>|<span data-ttu-id="2f9d3-118">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="2f9d3-119">删除</span><span class="sxs-lookup"><span data-stu-id="2f9d3-119">remove</span></span>|<span data-ttu-id="2f9d3-120">3</span><span class="sxs-lookup"><span data-stu-id="2f9d3-120">3</span></span>|<span data-ttu-id="2f9d3-121">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="2f9d3-122">允许</span><span class="sxs-lookup"><span data-stu-id="2f9d3-122">allow</span></span>|<span data-ttu-id="2f9d3-123">4</span><span class="sxs-lookup"><span data-stu-id="2f9d3-123">4</span></span>|<span data-ttu-id="2f9d3-124">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="2f9d3-125">用户定制</span><span class="sxs-lookup"><span data-stu-id="2f9d3-125">userDefined</span></span>|<span data-ttu-id="2f9d3-126">5</span><span class="sxs-lookup"><span data-stu-id="2f9d3-126">5</span></span>|<span data-ttu-id="2f9d3-127">允许用户以确定要使用的检测威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="2f9d3-128">阻止</span><span class="sxs-lookup"><span data-stu-id="2f9d3-128">block</span></span>|<span data-ttu-id="2f9d3-129">6</span><span class="sxs-lookup"><span data-stu-id="2f9d3-129">6</span></span>|<span data-ttu-id="2f9d3-130">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="2f9d3-130">Block the detected threat.</span></span>|



