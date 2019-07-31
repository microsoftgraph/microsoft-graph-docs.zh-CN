---
title: enrollmentState 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f394b02eac7e54c7e74a1c6954d6e3a7414e1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999183"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="dbcd8-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dbcd8-103">enrollmentState enum type</span></span>

> <span data-ttu-id="dbcd8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbcd8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbcd8-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dbcd8-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="dbcd8-107">成员</span><span class="sxs-lookup"><span data-stu-id="dbcd8-107">Members</span></span>
|<span data-ttu-id="dbcd8-108">成员</span><span class="sxs-lookup"><span data-stu-id="dbcd8-108">Member</span></span>|<span data-ttu-id="dbcd8-109">值</span><span class="sxs-lookup"><span data-stu-id="dbcd8-109">Value</span></span>|<span data-ttu-id="dbcd8-110">说明</span><span class="sxs-lookup"><span data-stu-id="dbcd8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbcd8-111">unknown</span><span class="sxs-lookup"><span data-stu-id="dbcd8-111">unknown</span></span>|<span data-ttu-id="dbcd8-112">0</span><span class="sxs-lookup"><span data-stu-id="dbcd8-112">0</span></span>|<span data-ttu-id="dbcd8-113">设备注册状态未知</span><span class="sxs-lookup"><span data-stu-id="dbcd8-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="dbcd8-114">注册</span><span class="sxs-lookup"><span data-stu-id="dbcd8-114">enrolled</span></span>|<span data-ttu-id="dbcd8-115">1</span><span class="sxs-lookup"><span data-stu-id="dbcd8-115">1</span></span>|<span data-ttu-id="dbcd8-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="dbcd8-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="dbcd8-117">pendingReset</span></span>|<span data-ttu-id="dbcd8-118">双面</span><span class="sxs-lookup"><span data-stu-id="dbcd8-118">2</span></span>|<span data-ttu-id="dbcd8-119">已注册, 但通过注册配置文件进行了注册, 并且注册的配置文件不同于分配的配置文件。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="dbcd8-120">未能</span><span class="sxs-lookup"><span data-stu-id="dbcd8-120">failed</span></span>|<span data-ttu-id="dbcd8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="dbcd8-121">3</span></span>|<span data-ttu-id="dbcd8-122">未注册, 并且存在注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="dbcd8-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="dbcd8-123">notContacted</span></span>|<span data-ttu-id="dbcd8-124">4</span><span class="sxs-lookup"><span data-stu-id="dbcd8-124">4</span></span>|<span data-ttu-id="dbcd8-125">导入了设备, 但未注册。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="dbcd8-126">堵塞</span><span class="sxs-lookup"><span data-stu-id="dbcd8-126">blocked</span></span>|<span data-ttu-id="dbcd8-127">5</span><span class="sxs-lookup"><span data-stu-id="dbcd8-127">5</span></span>|<span data-ttu-id="dbcd8-128">设备已注册为 userless, 但由于应用程序安装失败而被阻止移到用户注册。</span><span class="sxs-lookup"><span data-stu-id="dbcd8-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





