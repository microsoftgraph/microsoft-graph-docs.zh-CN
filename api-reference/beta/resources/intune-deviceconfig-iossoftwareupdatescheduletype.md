---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 04140e06bacb3602245eb84a34b9fa0ac11007fd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273576"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a><span data-ttu-id="453b9-103">iosSoftwareUpdateScheduleType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="453b9-103">iosSoftwareUpdateScheduleType enum type</span></span>

<span data-ttu-id="453b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="453b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="453b9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="453b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="453b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="453b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="453b9-107">更新 iOS 软件更新的计划类型。</span><span class="sxs-lookup"><span data-stu-id="453b9-107">Update schedule type for iOS software updates.</span></span>

## <a name="members"></a><span data-ttu-id="453b9-108">成员</span><span class="sxs-lookup"><span data-stu-id="453b9-108">Members</span></span>
|<span data-ttu-id="453b9-109">成员</span><span class="sxs-lookup"><span data-stu-id="453b9-109">Member</span></span>|<span data-ttu-id="453b9-110">值</span><span class="sxs-lookup"><span data-stu-id="453b9-110">Value</span></span>|<span data-ttu-id="453b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="453b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453b9-112">updateOutsideOfActiveHours</span><span class="sxs-lookup"><span data-stu-id="453b9-112">updateOutsideOfActiveHours</span></span>|<span data-ttu-id="453b9-113">0</span><span class="sxs-lookup"><span data-stu-id="453b9-113">0</span></span>|<span data-ttu-id="453b9-114">更新为主动时段之外的。</span><span class="sxs-lookup"><span data-stu-id="453b9-114">Update outside of active hours.</span></span>|
|<span data-ttu-id="453b9-115">alwaysUpdate</span><span class="sxs-lookup"><span data-stu-id="453b9-115">alwaysUpdate</span></span>|<span data-ttu-id="453b9-116">1</span><span class="sxs-lookup"><span data-stu-id="453b9-116">1</span></span>|<span data-ttu-id="453b9-117">时刻更新。</span><span class="sxs-lookup"><span data-stu-id="453b9-117">Always update.</span></span>|
|<span data-ttu-id="453b9-118">updateDuringTimeWindows</span><span class="sxs-lookup"><span data-stu-id="453b9-118">updateDuringTimeWindows</span></span>|<span data-ttu-id="453b9-119">双面</span><span class="sxs-lookup"><span data-stu-id="453b9-119">2</span></span>|<span data-ttu-id="453b9-120">在时间时段内更新。</span><span class="sxs-lookup"><span data-stu-id="453b9-120">Update during time windows.</span></span>|
|<span data-ttu-id="453b9-121">updateOutsideOfTimeWindows</span><span class="sxs-lookup"><span data-stu-id="453b9-121">updateOutsideOfTimeWindows</span></span>|<span data-ttu-id="453b9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="453b9-122">3</span></span>|<span data-ttu-id="453b9-123">在时段外更新。</span><span class="sxs-lookup"><span data-stu-id="453b9-123">Update outside of time windows.</span></span>|




