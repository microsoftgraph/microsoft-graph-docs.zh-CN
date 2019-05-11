---
title: enrollmentState 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78038fc9a279536c1e68708b767c6b7c81e4e4df
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941574"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="227ea-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="227ea-103">enrollmentState enum type</span></span>

> <span data-ttu-id="227ea-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="227ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="227ea-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="227ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="227ea-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="227ea-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="227ea-107">成员</span><span class="sxs-lookup"><span data-stu-id="227ea-107">Members</span></span>
|<span data-ttu-id="227ea-108">成员</span><span class="sxs-lookup"><span data-stu-id="227ea-108">Member</span></span>|<span data-ttu-id="227ea-109">值</span><span class="sxs-lookup"><span data-stu-id="227ea-109">Value</span></span>|<span data-ttu-id="227ea-110">说明</span><span class="sxs-lookup"><span data-stu-id="227ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227ea-111">unknown</span><span class="sxs-lookup"><span data-stu-id="227ea-111">unknown</span></span>|<span data-ttu-id="227ea-112">0</span><span class="sxs-lookup"><span data-stu-id="227ea-112">0</span></span>|<span data-ttu-id="227ea-113">设备注册状态未知</span><span class="sxs-lookup"><span data-stu-id="227ea-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="227ea-114">注册</span><span class="sxs-lookup"><span data-stu-id="227ea-114">enrolled</span></span>|<span data-ttu-id="227ea-115">1</span><span class="sxs-lookup"><span data-stu-id="227ea-115">1</span></span>|<span data-ttu-id="227ea-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="227ea-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="227ea-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="227ea-117">pendingReset</span></span>|<span data-ttu-id="227ea-118">双面</span><span class="sxs-lookup"><span data-stu-id="227ea-118">2</span></span>|<span data-ttu-id="227ea-119">已注册, 但通过注册配置文件进行了注册, 并且注册的配置文件不同于分配的配置文件。</span><span class="sxs-lookup"><span data-stu-id="227ea-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="227ea-120">未能</span><span class="sxs-lookup"><span data-stu-id="227ea-120">failed</span></span>|<span data-ttu-id="227ea-121">第三章</span><span class="sxs-lookup"><span data-stu-id="227ea-121">3</span></span>|<span data-ttu-id="227ea-122">未注册, 并且存在注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="227ea-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="227ea-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="227ea-123">notContacted</span></span>|<span data-ttu-id="227ea-124">4</span><span class="sxs-lookup"><span data-stu-id="227ea-124">4</span></span>|<span data-ttu-id="227ea-125">导入了设备, 但未注册。</span><span class="sxs-lookup"><span data-stu-id="227ea-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="227ea-126">堵塞</span><span class="sxs-lookup"><span data-stu-id="227ea-126">blocked</span></span>|<span data-ttu-id="227ea-127">5</span><span class="sxs-lookup"><span data-stu-id="227ea-127">5</span></span>|<span data-ttu-id="227ea-128">设备已注册为 userless, 但由于应用程序安装失败而被阻止移到用户注册。</span><span class="sxs-lookup"><span data-stu-id="227ea-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




