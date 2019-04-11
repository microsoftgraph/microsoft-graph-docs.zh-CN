---
title: managedAppFlaggedReason 枚举类型
description: 用户已被标记的原因
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf3190ce35d56ef83d19368001175896cb794c01
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772368"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="0573b-103">managedAppFlaggedReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0573b-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="0573b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0573b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0573b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0573b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0573b-106">用户已被标记的原因</span><span class="sxs-lookup"><span data-stu-id="0573b-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="0573b-107">成员</span><span class="sxs-lookup"><span data-stu-id="0573b-107">Members</span></span>
|<span data-ttu-id="0573b-108">成员</span><span class="sxs-lookup"><span data-stu-id="0573b-108">Member</span></span>|<span data-ttu-id="0573b-109">值</span><span class="sxs-lookup"><span data-stu-id="0573b-109">Value</span></span>|<span data-ttu-id="0573b-110">说明</span><span class="sxs-lookup"><span data-stu-id="0573b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0573b-111">无</span><span class="sxs-lookup"><span data-stu-id="0573b-111">none</span></span>|<span data-ttu-id="0573b-112">0</span><span class="sxs-lookup"><span data-stu-id="0573b-112">0</span></span>|<span data-ttu-id="0573b-113">无问题。</span><span class="sxs-lookup"><span data-stu-id="0573b-113">No issue.</span></span>|
|<span data-ttu-id="0573b-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="0573b-114">rootedDevice</span></span>|<span data-ttu-id="0573b-115">1</span><span class="sxs-lookup"><span data-stu-id="0573b-115">1</span></span>|<span data-ttu-id="0573b-116">应用注册在根/解锁设备上运行。</span><span class="sxs-lookup"><span data-stu-id="0573b-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="0573b-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="0573b-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="0573b-118">双面</span><span class="sxs-lookup"><span data-stu-id="0573b-118">2</span></span>|<span data-ttu-id="0573b-119">应用注册在解锁了启用程序的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="0573b-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="0573b-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="0573b-120">androidFactoryRomModified</span></span>|<span data-ttu-id="0573b-121">第三章</span><span class="sxs-lookup"><span data-stu-id="0573b-121">3</span></span>|<span data-ttu-id="0573b-122">应用注册在已修改出厂 ROM 的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="0573b-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





