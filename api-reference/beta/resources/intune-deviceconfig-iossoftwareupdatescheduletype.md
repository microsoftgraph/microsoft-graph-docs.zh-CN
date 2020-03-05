---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58a59e32fd75a99c9585d9c22115620b8a4aad20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526302"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a><span data-ttu-id="428ac-103">iosSoftwareUpdateScheduleType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="428ac-103">iosSoftwareUpdateScheduleType enum type</span></span>

<span data-ttu-id="428ac-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="428ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="428ac-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="428ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="428ac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="428ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="428ac-107">更新 iOS 软件更新的计划类型。</span><span class="sxs-lookup"><span data-stu-id="428ac-107">Update schedule type for iOS software updates.</span></span>

## <a name="members"></a><span data-ttu-id="428ac-108">成员</span><span class="sxs-lookup"><span data-stu-id="428ac-108">Members</span></span>
|<span data-ttu-id="428ac-109">成员</span><span class="sxs-lookup"><span data-stu-id="428ac-109">Member</span></span>|<span data-ttu-id="428ac-110">值</span><span class="sxs-lookup"><span data-stu-id="428ac-110">Value</span></span>|<span data-ttu-id="428ac-111">说明</span><span class="sxs-lookup"><span data-stu-id="428ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="428ac-112">updateOutsideOfActiveHours</span><span class="sxs-lookup"><span data-stu-id="428ac-112">updateOutsideOfActiveHours</span></span>|<span data-ttu-id="428ac-113">0</span><span class="sxs-lookup"><span data-stu-id="428ac-113">0</span></span>|<span data-ttu-id="428ac-114">更新为主动时段之外的。</span><span class="sxs-lookup"><span data-stu-id="428ac-114">Update outside of active hours.</span></span>|
|<span data-ttu-id="428ac-115">alwaysUpdate</span><span class="sxs-lookup"><span data-stu-id="428ac-115">alwaysUpdate</span></span>|<span data-ttu-id="428ac-116">1 </span><span class="sxs-lookup"><span data-stu-id="428ac-116">1</span></span>|<span data-ttu-id="428ac-117">时刻更新。</span><span class="sxs-lookup"><span data-stu-id="428ac-117">Always update.</span></span>|
|<span data-ttu-id="428ac-118">updateDuringTimeWindows</span><span class="sxs-lookup"><span data-stu-id="428ac-118">updateDuringTimeWindows</span></span>|<span data-ttu-id="428ac-119">2 </span><span class="sxs-lookup"><span data-stu-id="428ac-119">2</span></span>|<span data-ttu-id="428ac-120">在时间时段内更新。</span><span class="sxs-lookup"><span data-stu-id="428ac-120">Update during time windows.</span></span>|
|<span data-ttu-id="428ac-121">updateOutsideOfTimeWindows</span><span class="sxs-lookup"><span data-stu-id="428ac-121">updateOutsideOfTimeWindows</span></span>|<span data-ttu-id="428ac-122">3 </span><span class="sxs-lookup"><span data-stu-id="428ac-122">3</span></span>|<span data-ttu-id="428ac-123">在时段外更新。</span><span class="sxs-lookup"><span data-stu-id="428ac-123">Update outside of time windows.</span></span>|



