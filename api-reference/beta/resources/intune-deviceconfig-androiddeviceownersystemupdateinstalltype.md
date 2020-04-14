---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: 适用于 Android 设备所有者的系统更新类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b64de74146e6ee6ffe30416d03277919e06490d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402771"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="d1779-103">androidDeviceOwnerSystemUpdateInstallType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d1779-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

<span data-ttu-id="d1779-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1779-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1779-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1779-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1779-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1779-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1779-107">适用于 Android 设备所有者的系统更新类型。</span><span class="sxs-lookup"><span data-stu-id="d1779-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="d1779-108">成员</span><span class="sxs-lookup"><span data-stu-id="d1779-108">Members</span></span>
|<span data-ttu-id="d1779-109">成员</span><span class="sxs-lookup"><span data-stu-id="d1779-109">Member</span></span>|<span data-ttu-id="d1779-110">值</span><span class="sxs-lookup"><span data-stu-id="d1779-110">Value</span></span>|<span data-ttu-id="d1779-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1779-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1779-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d1779-112">deviceDefault</span></span>|<span data-ttu-id="d1779-113">0</span><span class="sxs-lookup"><span data-stu-id="d1779-113">0</span></span>|<span data-ttu-id="d1779-114">设备默认行为，通常提示用户接受系统更新。</span><span class="sxs-lookup"><span data-stu-id="d1779-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="d1779-115">推迟</span><span class="sxs-lookup"><span data-stu-id="d1779-115">postpone</span></span>|<span data-ttu-id="d1779-116">1</span><span class="sxs-lookup"><span data-stu-id="d1779-116">1</span></span>|<span data-ttu-id="d1779-117">将更新自动安装推迟30天。</span><span class="sxs-lookup"><span data-stu-id="d1779-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="d1779-118">开</span><span class="sxs-lookup"><span data-stu-id="d1779-118">windowed</span></span>|<span data-ttu-id="d1779-119">双面</span><span class="sxs-lookup"><span data-stu-id="d1779-119">2</span></span>|<span data-ttu-id="d1779-120">在每日维护时段内自动安装。</span><span class="sxs-lookup"><span data-stu-id="d1779-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="d1779-121">自动</span><span class="sxs-lookup"><span data-stu-id="d1779-121">automatic</span></span>|<span data-ttu-id="d1779-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d1779-122">3</span></span>|<span data-ttu-id="d1779-123">尽快自动安装更新。</span><span class="sxs-lookup"><span data-stu-id="d1779-123">Automatically install updates as soon as possible.</span></span>|



