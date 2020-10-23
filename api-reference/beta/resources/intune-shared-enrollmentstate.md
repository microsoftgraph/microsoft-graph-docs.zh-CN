---
title: enrollmentState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8f62798a99f93e6b4cb52bdac0d4681c4e06c5e9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735132"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="69240-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="69240-103">enrollmentState enum type</span></span>

<span data-ttu-id="69240-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69240-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69240-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69240-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69240-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69240-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69240-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="69240-108">成员</span><span class="sxs-lookup"><span data-stu-id="69240-108">Members</span></span>
|<span data-ttu-id="69240-109">成员</span><span class="sxs-lookup"><span data-stu-id="69240-109">Member</span></span>|<span data-ttu-id="69240-110">值</span><span class="sxs-lookup"><span data-stu-id="69240-110">Value</span></span>|<span data-ttu-id="69240-111">说明</span><span class="sxs-lookup"><span data-stu-id="69240-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69240-112">unknown</span><span class="sxs-lookup"><span data-stu-id="69240-112">unknown</span></span>|<span data-ttu-id="69240-113">0</span><span class="sxs-lookup"><span data-stu-id="69240-113">0</span></span>|<span data-ttu-id="69240-114">设备注册状态未知</span><span class="sxs-lookup"><span data-stu-id="69240-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="69240-115">注册</span><span class="sxs-lookup"><span data-stu-id="69240-115">enrolled</span></span>|<span data-ttu-id="69240-116">1</span><span class="sxs-lookup"><span data-stu-id="69240-116">1</span></span>|<span data-ttu-id="69240-117">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="69240-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="69240-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="69240-118">pendingReset</span></span>|<span data-ttu-id="69240-119">双面</span><span class="sxs-lookup"><span data-stu-id="69240-119">2</span></span>|<span data-ttu-id="69240-120">已注册，但通过注册配置文件进行了注册，并且注册的配置文件不同于分配的配置文件。</span><span class="sxs-lookup"><span data-stu-id="69240-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="69240-121">未能</span><span class="sxs-lookup"><span data-stu-id="69240-121">failed</span></span>|<span data-ttu-id="69240-122">第三章</span><span class="sxs-lookup"><span data-stu-id="69240-122">3</span></span>|<span data-ttu-id="69240-123">未注册，并且存在注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="69240-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="69240-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="69240-124">notContacted</span></span>|<span data-ttu-id="69240-125">4 </span><span class="sxs-lookup"><span data-stu-id="69240-125">4</span></span>|<span data-ttu-id="69240-126">导入了设备，但未注册。</span><span class="sxs-lookup"><span data-stu-id="69240-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="69240-127">堵塞</span><span class="sxs-lookup"><span data-stu-id="69240-127">blocked</span></span>|<span data-ttu-id="69240-128">5 </span><span class="sxs-lookup"><span data-stu-id="69240-128">5</span></span>|<span data-ttu-id="69240-129">设备已注册为 userless，但由于应用程序安装失败而被阻止移到用户注册。</span><span class="sxs-lookup"><span data-stu-id="69240-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





