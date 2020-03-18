---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: 适用于 Android 设备所有者的系统更新类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 043f1f22f4994950466e0f07288553d4c4adf101
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796970"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="800ec-103">androidDeviceOwnerSystemUpdateInstallType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="800ec-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="800ec-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="800ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="800ec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="800ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="800ec-106">适用于 Android 设备所有者的系统更新类型。</span><span class="sxs-lookup"><span data-stu-id="800ec-106">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="800ec-107">成员</span><span class="sxs-lookup"><span data-stu-id="800ec-107">Members</span></span>
|<span data-ttu-id="800ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="800ec-108">Member</span></span>|<span data-ttu-id="800ec-109">值</span><span class="sxs-lookup"><span data-stu-id="800ec-109">Value</span></span>|<span data-ttu-id="800ec-110">说明</span><span class="sxs-lookup"><span data-stu-id="800ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="800ec-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="800ec-111">deviceDefault</span></span>|<span data-ttu-id="800ec-112">0</span><span class="sxs-lookup"><span data-stu-id="800ec-112">0</span></span>|<span data-ttu-id="800ec-113">设备默认行为，通常提示用户接受系统更新。</span><span class="sxs-lookup"><span data-stu-id="800ec-113">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="800ec-114">推迟</span><span class="sxs-lookup"><span data-stu-id="800ec-114">postpone</span></span>|<span data-ttu-id="800ec-115">1</span><span class="sxs-lookup"><span data-stu-id="800ec-115">1</span></span>|<span data-ttu-id="800ec-116">将更新自动安装推迟30天。</span><span class="sxs-lookup"><span data-stu-id="800ec-116">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="800ec-117">开</span><span class="sxs-lookup"><span data-stu-id="800ec-117">windowed</span></span>|<span data-ttu-id="800ec-118">双面</span><span class="sxs-lookup"><span data-stu-id="800ec-118">2</span></span>|<span data-ttu-id="800ec-119">在每日维护时段内自动安装。</span><span class="sxs-lookup"><span data-stu-id="800ec-119">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="800ec-120">自动</span><span class="sxs-lookup"><span data-stu-id="800ec-120">automatic</span></span>|<span data-ttu-id="800ec-121">第三章</span><span class="sxs-lookup"><span data-stu-id="800ec-121">3</span></span>|<span data-ttu-id="800ec-122">尽快自动安装更新。</span><span class="sxs-lookup"><span data-stu-id="800ec-122">Automatically install updates as soon as possible.</span></span>|



