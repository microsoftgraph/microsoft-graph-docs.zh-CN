---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: 适用于 Android 设备所有者的系统更新类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 509f31187e46f12c039ce5172722003fccd2e786
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685441"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="3ceb7-103">androidDeviceOwnerSystemUpdateInstallType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3ceb7-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

<span data-ttu-id="3ceb7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ceb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ceb7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ceb7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ceb7-107">适用于 Android 设备所有者的系统更新类型。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="3ceb7-108">成员</span><span class="sxs-lookup"><span data-stu-id="3ceb7-108">Members</span></span>
|<span data-ttu-id="3ceb7-109">成员</span><span class="sxs-lookup"><span data-stu-id="3ceb7-109">Member</span></span>|<span data-ttu-id="3ceb7-110">值</span><span class="sxs-lookup"><span data-stu-id="3ceb7-110">Value</span></span>|<span data-ttu-id="3ceb7-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ceb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ceb7-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3ceb7-112">deviceDefault</span></span>|<span data-ttu-id="3ceb7-113">0</span><span class="sxs-lookup"><span data-stu-id="3ceb7-113">0</span></span>|<span data-ttu-id="3ceb7-114">设备默认行为，通常提示用户接受系统更新。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="3ceb7-115">推迟</span><span class="sxs-lookup"><span data-stu-id="3ceb7-115">postpone</span></span>|<span data-ttu-id="3ceb7-116">1</span><span class="sxs-lookup"><span data-stu-id="3ceb7-116">1</span></span>|<span data-ttu-id="3ceb7-117">将更新自动安装推迟30天。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="3ceb7-118">开</span><span class="sxs-lookup"><span data-stu-id="3ceb7-118">windowed</span></span>|<span data-ttu-id="3ceb7-119">双面</span><span class="sxs-lookup"><span data-stu-id="3ceb7-119">2</span></span>|<span data-ttu-id="3ceb7-120">在每日维护时段内自动安装。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="3ceb7-121">自动</span><span class="sxs-lookup"><span data-stu-id="3ceb7-121">automatic</span></span>|<span data-ttu-id="3ceb7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="3ceb7-122">3</span></span>|<span data-ttu-id="3ceb7-123">尽快自动安装更新。</span><span class="sxs-lookup"><span data-stu-id="3ceb7-123">Automatically install updates as soon as possible.</span></span>|





