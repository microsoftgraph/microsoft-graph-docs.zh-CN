---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923941"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="e402f-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e402f-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="e402f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e402f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e402f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e402f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e402f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e402f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e402f-107">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="e402f-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="e402f-108">成员</span><span class="sxs-lookup"><span data-stu-id="e402f-108">Members</span></span>
|<span data-ttu-id="e402f-109">成员</span><span class="sxs-lookup"><span data-stu-id="e402f-109">Member</span></span>|<span data-ttu-id="e402f-110">值</span><span class="sxs-lookup"><span data-stu-id="e402f-110">Value</span></span>|<span data-ttu-id="e402f-111">Description</span><span class="sxs-lookup"><span data-stu-id="e402f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e402f-112">clean</span><span class="sxs-lookup"><span data-stu-id="e402f-112">clean</span></span>|<span data-ttu-id="e402f-113">0</span><span class="sxs-lookup"><span data-stu-id="e402f-113">0</span></span>|<span data-ttu-id="e402f-114">计算机的完全而不不需要任何操作</span><span class="sxs-lookup"><span data-stu-id="e402f-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="e402f-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="e402f-115">fullScanPending</span></span>|<span data-ttu-id="e402f-116">1</span><span class="sxs-lookup"><span data-stu-id="e402f-116">1</span></span>|<span data-ttu-id="e402f-117">计算机处于挂起完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="e402f-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="e402f-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="e402f-118">rebootPending</span></span>|<span data-ttu-id="e402f-119">2</span><span class="sxs-lookup"><span data-stu-id="e402f-119">2</span></span>|<span data-ttu-id="e402f-120">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="e402f-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="e402f-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="e402f-121">manualStepsPending</span></span>|<span data-ttu-id="e402f-122">4</span><span class="sxs-lookup"><span data-stu-id="e402f-122">4</span></span>|<span data-ttu-id="e402f-123">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="e402f-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="e402f-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="e402f-124">offlineScanPending</span></span>|<span data-ttu-id="e402f-125">8</span><span class="sxs-lookup"><span data-stu-id="e402f-125">8</span></span>|<span data-ttu-id="e402f-126">计算机处于挂起脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="e402f-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="e402f-127">critical</span><span class="sxs-lookup"><span data-stu-id="e402f-127">critical</span></span>|<span data-ttu-id="e402f-128">16</span><span class="sxs-lookup"><span data-stu-id="e402f-128">16</span></span>|<span data-ttu-id="e402f-129">计算机处于关键失败状态</span><span class="sxs-lookup"><span data-stu-id="e402f-129">Computer is in critical failure state</span></span>|





