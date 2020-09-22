---
title: enrollmentState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: da96d5e0f1b86057178755bbd4e0761f49220095
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084294"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="5150a-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5150a-103">enrollmentState enum type</span></span>

<span data-ttu-id="5150a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5150a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5150a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5150a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5150a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5150a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5150a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5150a-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="5150a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5150a-108">Members</span></span>
|<span data-ttu-id="5150a-109">成员</span><span class="sxs-lookup"><span data-stu-id="5150a-109">Member</span></span>|<span data-ttu-id="5150a-110">值</span><span class="sxs-lookup"><span data-stu-id="5150a-110">Value</span></span>|<span data-ttu-id="5150a-111">说明</span><span class="sxs-lookup"><span data-stu-id="5150a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5150a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5150a-112">unknown</span></span>|<span data-ttu-id="5150a-113">0</span><span class="sxs-lookup"><span data-stu-id="5150a-113">0</span></span>|<span data-ttu-id="5150a-114">设备注册状态未知</span><span class="sxs-lookup"><span data-stu-id="5150a-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="5150a-115">注册</span><span class="sxs-lookup"><span data-stu-id="5150a-115">enrolled</span></span>|<span data-ttu-id="5150a-116">1 </span><span class="sxs-lookup"><span data-stu-id="5150a-116">1</span></span>|<span data-ttu-id="5150a-117">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="5150a-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="5150a-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="5150a-118">pendingReset</span></span>|<span data-ttu-id="5150a-119">2 </span><span class="sxs-lookup"><span data-stu-id="5150a-119">2</span></span>|<span data-ttu-id="5150a-120">已注册，但通过注册配置文件进行了注册，并且注册的配置文件不同于分配的配置文件。</span><span class="sxs-lookup"><span data-stu-id="5150a-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="5150a-121">未能</span><span class="sxs-lookup"><span data-stu-id="5150a-121">failed</span></span>|<span data-ttu-id="5150a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="5150a-122">3</span></span>|<span data-ttu-id="5150a-123">未注册，并且存在注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="5150a-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="5150a-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="5150a-124">notContacted</span></span>|<span data-ttu-id="5150a-125">4 </span><span class="sxs-lookup"><span data-stu-id="5150a-125">4</span></span>|<span data-ttu-id="5150a-126">导入了设备，但未注册。</span><span class="sxs-lookup"><span data-stu-id="5150a-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="5150a-127">堵塞</span><span class="sxs-lookup"><span data-stu-id="5150a-127">blocked</span></span>|<span data-ttu-id="5150a-128">5 </span><span class="sxs-lookup"><span data-stu-id="5150a-128">5</span></span>|<span data-ttu-id="5150a-129">设备已注册为 userless，但由于应用程序安装失败而被阻止移到用户注册。</span><span class="sxs-lookup"><span data-stu-id="5150a-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|






