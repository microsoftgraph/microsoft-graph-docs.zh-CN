---
title: macOSSoftwareUpdateScheduleType 枚举类型
description: 更新 macOS 软件更新的计划类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 314b07f7a689bc98c4e1b714c29c23f85dd37b67
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294002"
---
# <a name="macossoftwareupdatescheduletype-enum-type"></a><span data-ttu-id="51f0c-103">macOSSoftwareUpdateScheduleType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="51f0c-103">macOSSoftwareUpdateScheduleType enum type</span></span>

<span data-ttu-id="51f0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51f0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51f0c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51f0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51f0c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51f0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51f0c-107">更新 macOS 软件更新的计划类型。</span><span class="sxs-lookup"><span data-stu-id="51f0c-107">Update schedule type for macOS software updates.</span></span>

## <a name="members"></a><span data-ttu-id="51f0c-108">成员</span><span class="sxs-lookup"><span data-stu-id="51f0c-108">Members</span></span>
|<span data-ttu-id="51f0c-109">成员</span><span class="sxs-lookup"><span data-stu-id="51f0c-109">Member</span></span>|<span data-ttu-id="51f0c-110">值</span><span class="sxs-lookup"><span data-stu-id="51f0c-110">Value</span></span>|<span data-ttu-id="51f0c-111">Description</span><span class="sxs-lookup"><span data-stu-id="51f0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51f0c-112">alwaysUpdate</span><span class="sxs-lookup"><span data-stu-id="51f0c-112">alwaysUpdate</span></span>|<span data-ttu-id="51f0c-113">0</span><span class="sxs-lookup"><span data-stu-id="51f0c-113">0</span></span>|<span data-ttu-id="51f0c-114">时刻更新。</span><span class="sxs-lookup"><span data-stu-id="51f0c-114">Always update.</span></span>|
|<span data-ttu-id="51f0c-115">updateDuringTimeWindows</span><span class="sxs-lookup"><span data-stu-id="51f0c-115">updateDuringTimeWindows</span></span>|<span data-ttu-id="51f0c-116">1</span><span class="sxs-lookup"><span data-stu-id="51f0c-116">1</span></span>|<span data-ttu-id="51f0c-117">在时间时段内更新。</span><span class="sxs-lookup"><span data-stu-id="51f0c-117">Update during time windows.</span></span>|
|<span data-ttu-id="51f0c-118">updateOutsideOfTimeWindows</span><span class="sxs-lookup"><span data-stu-id="51f0c-118">updateOutsideOfTimeWindows</span></span>|<span data-ttu-id="51f0c-119">双面</span><span class="sxs-lookup"><span data-stu-id="51f0c-119">2</span></span>|<span data-ttu-id="51f0c-120">在时段外更新。</span><span class="sxs-lookup"><span data-stu-id="51f0c-120">Update outside of time windows.</span></span>|




