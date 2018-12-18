---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
author: tfitzmac
ms.openlocfilehash: b794f8121132e396459f9198c644084690fe95b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326325"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="f6e55-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f6e55-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="f6e55-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f6e55-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6e55-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6e55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6e55-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f6e55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6e55-107">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="f6e55-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="f6e55-108">成员</span><span class="sxs-lookup"><span data-stu-id="f6e55-108">Members</span></span>
|<span data-ttu-id="f6e55-109">成员</span><span class="sxs-lookup"><span data-stu-id="f6e55-109">Member</span></span>|<span data-ttu-id="f6e55-110">值</span><span class="sxs-lookup"><span data-stu-id="f6e55-110">Value</span></span>|<span data-ttu-id="f6e55-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6e55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e55-112">clean</span><span class="sxs-lookup"><span data-stu-id="f6e55-112">clean</span></span>|<span data-ttu-id="f6e55-113">0</span><span class="sxs-lookup"><span data-stu-id="f6e55-113">0</span></span>|<span data-ttu-id="f6e55-114">计算机的完全而不不需要任何操作</span><span class="sxs-lookup"><span data-stu-id="f6e55-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="f6e55-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="f6e55-115">fullScanPending</span></span>|<span data-ttu-id="f6e55-116">1</span><span class="sxs-lookup"><span data-stu-id="f6e55-116">1</span></span>|<span data-ttu-id="f6e55-117">计算机处于挂起完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="f6e55-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="f6e55-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="f6e55-118">rebootPending</span></span>|<span data-ttu-id="f6e55-119">2</span><span class="sxs-lookup"><span data-stu-id="f6e55-119">2</span></span>|<span data-ttu-id="f6e55-120">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="f6e55-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="f6e55-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="f6e55-121">manualStepsPending</span></span>|<span data-ttu-id="f6e55-122">4</span><span class="sxs-lookup"><span data-stu-id="f6e55-122">4</span></span>|<span data-ttu-id="f6e55-123">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="f6e55-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="f6e55-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="f6e55-124">offlineScanPending</span></span>|<span data-ttu-id="f6e55-125">8</span><span class="sxs-lookup"><span data-stu-id="f6e55-125">8</span></span>|<span data-ttu-id="f6e55-126">计算机处于挂起脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="f6e55-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="f6e55-127">critical</span><span class="sxs-lookup"><span data-stu-id="f6e55-127">critical</span></span>|<span data-ttu-id="f6e55-128">16</span><span class="sxs-lookup"><span data-stu-id="f6e55-128">16</span></span>|<span data-ttu-id="f6e55-129">计算机处于关键失败状态</span><span class="sxs-lookup"><span data-stu-id="f6e55-129">Computer is in critical failure state</span></span>|





