---
title: defenderThreatAction 枚举类型
description: Defender 对检测到的恶意软件威胁采取的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 636d20b3c71b62157946e77230cd8945dd9957cd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758888"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="8cc09-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8cc09-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="8cc09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc09-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8cc09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc09-106">Defender 对检测到的恶意软件威胁采取的默认操作。</span><span class="sxs-lookup"><span data-stu-id="8cc09-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="8cc09-107">成员</span><span class="sxs-lookup"><span data-stu-id="8cc09-107">Members</span></span>
|<span data-ttu-id="8cc09-108">成员</span><span class="sxs-lookup"><span data-stu-id="8cc09-108">Member</span></span>|<span data-ttu-id="8cc09-109">值</span><span class="sxs-lookup"><span data-stu-id="8cc09-109">Value</span></span>|<span data-ttu-id="8cc09-110">说明</span><span class="sxs-lookup"><span data-stu-id="8cc09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc09-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8cc09-111">deviceDefault</span></span>|<span data-ttu-id="8cc09-112">0</span><span class="sxs-lookup"><span data-stu-id="8cc09-112">0</span></span>|<span data-ttu-id="8cc09-113">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="8cc09-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="8cc09-114">clean</span><span class="sxs-lookup"><span data-stu-id="8cc09-114">clean</span></span>|<span data-ttu-id="8cc09-115">1</span><span class="sxs-lookup"><span data-stu-id="8cc09-115">1</span></span>|<span data-ttu-id="8cc09-116">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="8cc09-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="8cc09-117">隔离</span><span class="sxs-lookup"><span data-stu-id="8cc09-117">quarantine</span></span>|<span data-ttu-id="8cc09-118">2</span><span class="sxs-lookup"><span data-stu-id="8cc09-118">2</span></span>|<span data-ttu-id="8cc09-119">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="8cc09-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="8cc09-120">remove</span><span class="sxs-lookup"><span data-stu-id="8cc09-120">remove</span></span>|<span data-ttu-id="8cc09-121">3</span><span class="sxs-lookup"><span data-stu-id="8cc09-121">3</span></span>|<span data-ttu-id="8cc09-122">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="8cc09-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="8cc09-123">allow</span><span class="sxs-lookup"><span data-stu-id="8cc09-123">allow</span></span>|<span data-ttu-id="8cc09-124">4 </span><span class="sxs-lookup"><span data-stu-id="8cc09-124">4</span></span>|<span data-ttu-id="8cc09-125">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="8cc09-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="8cc09-126">userDefined</span><span class="sxs-lookup"><span data-stu-id="8cc09-126">userDefined</span></span>|<span data-ttu-id="8cc09-127">5 </span><span class="sxs-lookup"><span data-stu-id="8cc09-127">5</span></span>|<span data-ttu-id="8cc09-128">允许用户确定对检测到的威胁要采取的操作。</span><span class="sxs-lookup"><span data-stu-id="8cc09-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="8cc09-129">block</span><span class="sxs-lookup"><span data-stu-id="8cc09-129">block</span></span>|<span data-ttu-id="8cc09-130">6 </span><span class="sxs-lookup"><span data-stu-id="8cc09-130">6</span></span>|<span data-ttu-id="8cc09-131">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="8cc09-131">Block the detected threat.</span></span>|




