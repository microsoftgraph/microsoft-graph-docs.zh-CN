---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: 适用于 Android 设备所有者的系统更新类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86f5e5d2c698652e7155c300fdd51e50442a1c44
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777002"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="b4a25-103">androidDeviceOwnerSystemUpdateInstallType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4a25-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="b4a25-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4a25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4a25-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4a25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4a25-106">适用于 Android 设备所有者的系统更新类型。</span><span class="sxs-lookup"><span data-stu-id="b4a25-106">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="b4a25-107">成员</span><span class="sxs-lookup"><span data-stu-id="b4a25-107">Members</span></span>
|<span data-ttu-id="b4a25-108">成员</span><span class="sxs-lookup"><span data-stu-id="b4a25-108">Member</span></span>|<span data-ttu-id="b4a25-109">值</span><span class="sxs-lookup"><span data-stu-id="b4a25-109">Value</span></span>|<span data-ttu-id="b4a25-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4a25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4a25-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b4a25-111">deviceDefault</span></span>|<span data-ttu-id="b4a25-112">0</span><span class="sxs-lookup"><span data-stu-id="b4a25-112">0</span></span>|<span data-ttu-id="b4a25-113">设备默认行为, 通常提示用户接受系统更新。</span><span class="sxs-lookup"><span data-stu-id="b4a25-113">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="b4a25-114">推迟</span><span class="sxs-lookup"><span data-stu-id="b4a25-114">postpone</span></span>|<span data-ttu-id="b4a25-115">1</span><span class="sxs-lookup"><span data-stu-id="b4a25-115">1</span></span>|<span data-ttu-id="b4a25-116">将更新自动安装推迟30天。</span><span class="sxs-lookup"><span data-stu-id="b4a25-116">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="b4a25-117">开</span><span class="sxs-lookup"><span data-stu-id="b4a25-117">windowed</span></span>|<span data-ttu-id="b4a25-118">双面</span><span class="sxs-lookup"><span data-stu-id="b4a25-118">2</span></span>|<span data-ttu-id="b4a25-119">在每日维护时段内自动安装。</span><span class="sxs-lookup"><span data-stu-id="b4a25-119">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="b4a25-120">自动</span><span class="sxs-lookup"><span data-stu-id="b4a25-120">automatic</span></span>|<span data-ttu-id="b4a25-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b4a25-121">3</span></span>|<span data-ttu-id="b4a25-122">尽快自动安装更新。</span><span class="sxs-lookup"><span data-stu-id="b4a25-122">Automatically install updates as soon as possible.</span></span>|





