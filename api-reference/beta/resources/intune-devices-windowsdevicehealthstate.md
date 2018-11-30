---
title: windowsDeviceHealthState 枚举类型
description: 计算机终结点保护状态
ms.openlocfilehash: 601531dd71ee0d44e9f5ebc89eb018ba5e0f2675
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041340"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="2dcd4-103">windowsDeviceHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2dcd4-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="2dcd4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2dcd4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dcd4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2dcd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2dcd4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2dcd4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dcd4-107">计算机终结点保护状态</span><span class="sxs-lookup"><span data-stu-id="2dcd4-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="2dcd4-108">成员</span><span class="sxs-lookup"><span data-stu-id="2dcd4-108">Members</span></span>
|<span data-ttu-id="2dcd4-109">成员</span><span class="sxs-lookup"><span data-stu-id="2dcd4-109">Member</span></span>|<span data-ttu-id="2dcd4-110">值</span><span class="sxs-lookup"><span data-stu-id="2dcd4-110">Value</span></span>|<span data-ttu-id="2dcd4-111">说明</span><span class="sxs-lookup"><span data-stu-id="2dcd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dcd4-112">clean</span><span class="sxs-lookup"><span data-stu-id="2dcd4-112">clean</span></span>|<span data-ttu-id="2dcd4-113">0</span><span class="sxs-lookup"><span data-stu-id="2dcd4-113">0</span></span>|<span data-ttu-id="2dcd4-114">计算机的完全而不不需要任何操作</span><span class="sxs-lookup"><span data-stu-id="2dcd4-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="2dcd4-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="2dcd4-115">fullScanPending</span></span>|<span data-ttu-id="2dcd4-116">1</span><span class="sxs-lookup"><span data-stu-id="2dcd4-116">1</span></span>|<span data-ttu-id="2dcd4-117">计算机处于挂起完全扫描状态</span><span class="sxs-lookup"><span data-stu-id="2dcd4-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="2dcd4-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="2dcd4-118">rebootPending</span></span>|<span data-ttu-id="2dcd4-119">2</span><span class="sxs-lookup"><span data-stu-id="2dcd4-119">2</span></span>|<span data-ttu-id="2dcd4-120">计算机处于挂起的重新启动状态</span><span class="sxs-lookup"><span data-stu-id="2dcd4-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="2dcd4-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="2dcd4-121">manualStepsPending</span></span>|<span data-ttu-id="2dcd4-122">4</span><span class="sxs-lookup"><span data-stu-id="2dcd4-122">4</span></span>|<span data-ttu-id="2dcd4-123">计算机处于挂起的手动步骤状态</span><span class="sxs-lookup"><span data-stu-id="2dcd4-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="2dcd4-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="2dcd4-124">offlineScanPending</span></span>|<span data-ttu-id="2dcd4-125">8</span><span class="sxs-lookup"><span data-stu-id="2dcd4-125">8</span></span>|<span data-ttu-id="2dcd4-126">计算机处于挂起脱机扫描状态</span><span class="sxs-lookup"><span data-stu-id="2dcd4-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="2dcd4-127">critical</span><span class="sxs-lookup"><span data-stu-id="2dcd4-127">critical</span></span>|<span data-ttu-id="2dcd4-128">16</span><span class="sxs-lookup"><span data-stu-id="2dcd4-128">16</span></span>|<span data-ttu-id="2dcd4-129">计算机处于关键失败状态</span><span class="sxs-lookup"><span data-stu-id="2dcd4-129">Computer is in critical failure state</span></span>|





