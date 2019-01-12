---
title: enrollmentState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9394755c5b6e6de8ed039b226d03074f1ef16cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933587"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="85e5f-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="85e5f-103">enrollmentState enum type</span></span>

> <span data-ttu-id="85e5f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85e5f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85e5f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85e5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85e5f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="85e5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85e5f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85e5f-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="85e5f-108">成员</span><span class="sxs-lookup"><span data-stu-id="85e5f-108">Members</span></span>
|<span data-ttu-id="85e5f-109">成员</span><span class="sxs-lookup"><span data-stu-id="85e5f-109">Member</span></span>|<span data-ttu-id="85e5f-110">值</span><span class="sxs-lookup"><span data-stu-id="85e5f-110">Value</span></span>|<span data-ttu-id="85e5f-111">Description</span><span class="sxs-lookup"><span data-stu-id="85e5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e5f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="85e5f-112">unknown</span></span>|<span data-ttu-id="85e5f-113">0</span><span class="sxs-lookup"><span data-stu-id="85e5f-113">0</span></span>|<span data-ttu-id="85e5f-114">设备注册状态是未知</span><span class="sxs-lookup"><span data-stu-id="85e5f-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="85e5f-115">注册</span><span class="sxs-lookup"><span data-stu-id="85e5f-115">enrolled</span></span>|<span data-ttu-id="85e5f-116">1</span><span class="sxs-lookup"><span data-stu-id="85e5f-116">1</span></span>|<span data-ttu-id="85e5f-117">注册设备。</span><span class="sxs-lookup"><span data-stu-id="85e5f-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="85e5f-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="85e5f-118">pendingReset</span></span>|<span data-ttu-id="85e5f-119">2</span><span class="sxs-lookup"><span data-stu-id="85e5f-119">2</span></span>|<span data-ttu-id="85e5f-120">注册但它通过注册配置文件中注册的注册的配置文件是不同的已分配的配置文件。</span><span class="sxs-lookup"><span data-stu-id="85e5f-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="85e5f-121">failed</span><span class="sxs-lookup"><span data-stu-id="85e5f-121">failed</span></span>|<span data-ttu-id="85e5f-122">3</span><span class="sxs-lookup"><span data-stu-id="85e5f-122">3</span></span>|<span data-ttu-id="85e5f-123">未注册，并且没有注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="85e5f-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="85e5f-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="85e5f-124">notContacted</span></span>|<span data-ttu-id="85e5f-125">4</span><span class="sxs-lookup"><span data-stu-id="85e5f-125">4</span></span>|<span data-ttu-id="85e5f-126">导入但未注册设备。</span><span class="sxs-lookup"><span data-stu-id="85e5f-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="85e5f-127">已阻止</span><span class="sxs-lookup"><span data-stu-id="85e5f-127">blocked</span></span>|<span data-ttu-id="85e5f-128">5</span><span class="sxs-lookup"><span data-stu-id="85e5f-128">5</span></span>|<span data-ttu-id="85e5f-129">设备注册为 userless，但阻止移动到用户注册，因为应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="85e5f-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





