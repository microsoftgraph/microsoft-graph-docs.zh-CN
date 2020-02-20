---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 431afa07b2276219186c508b88bc05ab981f65ff
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162426"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a><span data-ttu-id="d6030-103">iosSoftwareUpdateScheduleType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d6030-103">iosSoftwareUpdateScheduleType enum type</span></span>

> <span data-ttu-id="d6030-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6030-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6030-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6030-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6030-106">更新 iOS 软件更新的计划类型。</span><span class="sxs-lookup"><span data-stu-id="d6030-106">Update schedule type for iOS software updates.</span></span>

## <a name="members"></a><span data-ttu-id="d6030-107">成员</span><span class="sxs-lookup"><span data-stu-id="d6030-107">Members</span></span>
|<span data-ttu-id="d6030-108">成员</span><span class="sxs-lookup"><span data-stu-id="d6030-108">Member</span></span>|<span data-ttu-id="d6030-109">值</span><span class="sxs-lookup"><span data-stu-id="d6030-109">Value</span></span>|<span data-ttu-id="d6030-110">说明</span><span class="sxs-lookup"><span data-stu-id="d6030-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6030-111">updateOutsideOfActiveHours</span><span class="sxs-lookup"><span data-stu-id="d6030-111">updateOutsideOfActiveHours</span></span>|<span data-ttu-id="d6030-112">0</span><span class="sxs-lookup"><span data-stu-id="d6030-112">0</span></span>|<span data-ttu-id="d6030-113">更新为主动时段之外的。</span><span class="sxs-lookup"><span data-stu-id="d6030-113">Update outside of active hours.</span></span>|
|<span data-ttu-id="d6030-114">alwaysUpdate</span><span class="sxs-lookup"><span data-stu-id="d6030-114">alwaysUpdate</span></span>|<span data-ttu-id="d6030-115">1</span><span class="sxs-lookup"><span data-stu-id="d6030-115">1</span></span>|<span data-ttu-id="d6030-116">时刻更新。</span><span class="sxs-lookup"><span data-stu-id="d6030-116">Always update.</span></span>|
|<span data-ttu-id="d6030-117">updateDuringTimeWindows</span><span class="sxs-lookup"><span data-stu-id="d6030-117">updateDuringTimeWindows</span></span>|<span data-ttu-id="d6030-118">双面</span><span class="sxs-lookup"><span data-stu-id="d6030-118">2</span></span>|<span data-ttu-id="d6030-119">在时间时段内更新。</span><span class="sxs-lookup"><span data-stu-id="d6030-119">Update during time windows.</span></span>|
|<span data-ttu-id="d6030-120">updateOutsideOfTimeWindows</span><span class="sxs-lookup"><span data-stu-id="d6030-120">updateOutsideOfTimeWindows</span></span>|<span data-ttu-id="d6030-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d6030-121">3</span></span>|<span data-ttu-id="d6030-122">在时段外更新。</span><span class="sxs-lookup"><span data-stu-id="d6030-122">Update outside of time windows.</span></span>|



