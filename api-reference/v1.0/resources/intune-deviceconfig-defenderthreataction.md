---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0195176f322230b3164856575880b9dadc24bce0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031778"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="9f3fa-103">defenderThreatAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9f3fa-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="9f3fa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f3fa-105">要对检测到的恶意软件威胁执行的 Defender 的默认操作。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="9f3fa-106">成员</span><span class="sxs-lookup"><span data-stu-id="9f3fa-106">Members</span></span>
|<span data-ttu-id="9f3fa-107">成员</span><span class="sxs-lookup"><span data-stu-id="9f3fa-107">Member</span></span>|<span data-ttu-id="9f3fa-108">值</span><span class="sxs-lookup"><span data-stu-id="9f3fa-108">Value</span></span>|<span data-ttu-id="9f3fa-109">说明</span><span class="sxs-lookup"><span data-stu-id="9f3fa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f3fa-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9f3fa-110">deviceDefault</span></span>|<span data-ttu-id="9f3fa-111">0</span><span class="sxs-lookup"><span data-stu-id="9f3fa-111">0</span></span>|<span data-ttu-id="9f3fa-112">根据更新定义应用操作。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="9f3fa-113">清理</span><span class="sxs-lookup"><span data-stu-id="9f3fa-113">clean</span></span>|<span data-ttu-id="9f3fa-114">1</span><span class="sxs-lookup"><span data-stu-id="9f3fa-114">1</span></span>|<span data-ttu-id="9f3fa-115">清理检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="9f3fa-116">隔离</span><span class="sxs-lookup"><span data-stu-id="9f3fa-116">quarantine</span></span>|<span data-ttu-id="9f3fa-117">双面</span><span class="sxs-lookup"><span data-stu-id="9f3fa-117">2</span></span>|<span data-ttu-id="9f3fa-118">隔离检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="9f3fa-119">删除</span><span class="sxs-lookup"><span data-stu-id="9f3fa-119">remove</span></span>|<span data-ttu-id="9f3fa-120">第三章</span><span class="sxs-lookup"><span data-stu-id="9f3fa-120">3</span></span>|<span data-ttu-id="9f3fa-121">删除检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="9f3fa-122">允许</span><span class="sxs-lookup"><span data-stu-id="9f3fa-122">allow</span></span>|<span data-ttu-id="9f3fa-123">4</span><span class="sxs-lookup"><span data-stu-id="9f3fa-123">4</span></span>|<span data-ttu-id="9f3fa-124">允许检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="9f3fa-125">定制</span><span class="sxs-lookup"><span data-stu-id="9f3fa-125">userDefined</span></span>|<span data-ttu-id="9f3fa-126">5</span><span class="sxs-lookup"><span data-stu-id="9f3fa-126">5</span></span>|<span data-ttu-id="9f3fa-127">允许用户确定要对检测到的威胁采取的操作。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="9f3fa-128">数据</span><span class="sxs-lookup"><span data-stu-id="9f3fa-128">block</span></span>|<span data-ttu-id="9f3fa-129">型</span><span class="sxs-lookup"><span data-stu-id="9f3fa-129">6</span></span>|<span data-ttu-id="9f3fa-130">阻止检测到的威胁。</span><span class="sxs-lookup"><span data-stu-id="9f3fa-130">Block the detected threat.</span></span>|



