---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534316"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="d184e-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d184e-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="d184e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d184e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d184e-105">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="d184e-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="d184e-106">成员</span><span class="sxs-lookup"><span data-stu-id="d184e-106">Members</span></span>
|<span data-ttu-id="d184e-107">成员</span><span class="sxs-lookup"><span data-stu-id="d184e-107">Member</span></span>|<span data-ttu-id="d184e-108">值</span><span class="sxs-lookup"><span data-stu-id="d184e-108">Value</span></span>|<span data-ttu-id="d184e-109">说明</span><span class="sxs-lookup"><span data-stu-id="d184e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d184e-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d184e-110">deviceDefault</span></span>|<span data-ttu-id="d184e-111">0</span><span class="sxs-lookup"><span data-stu-id="d184e-111">0</span></span>|<span data-ttu-id="d184e-112">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="d184e-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="d184e-113">清理</span><span class="sxs-lookup"><span data-stu-id="d184e-113">clean</span></span>|<span data-ttu-id="d184e-114">1</span><span class="sxs-lookup"><span data-stu-id="d184e-114">1</span></span>|<span data-ttu-id="d184e-115">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d184e-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="d184e-116">隔离</span><span class="sxs-lookup"><span data-stu-id="d184e-116">quarantine</span></span>|<span data-ttu-id="d184e-117">2 </span><span class="sxs-lookup"><span data-stu-id="d184e-117">2</span></span>|<span data-ttu-id="d184e-118">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d184e-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="d184e-119">删除</span><span class="sxs-lookup"><span data-stu-id="d184e-119">remove</span></span>|<span data-ttu-id="d184e-120">3 </span><span class="sxs-lookup"><span data-stu-id="d184e-120">3</span></span>|<span data-ttu-id="d184e-121">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d184e-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="d184e-122">允许</span><span class="sxs-lookup"><span data-stu-id="d184e-122">allow</span></span>|<span data-ttu-id="d184e-123">4 </span><span class="sxs-lookup"><span data-stu-id="d184e-123">4</span></span>|<span data-ttu-id="d184e-124">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d184e-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="d184e-125">定制</span><span class="sxs-lookup"><span data-stu-id="d184e-125">userDefined</span></span>|<span data-ttu-id="d184e-126">5 </span><span class="sxs-lookup"><span data-stu-id="d184e-126">5</span></span>|<span data-ttu-id="d184e-127">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="d184e-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="d184e-128">数据</span><span class="sxs-lookup"><span data-stu-id="d184e-128">block</span></span>|<span data-ttu-id="d184e-129">6 </span><span class="sxs-lookup"><span data-stu-id="d184e-129">6</span></span>|<span data-ttu-id="d184e-130">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="d184e-130">Block the detected threat.</span></span>|



