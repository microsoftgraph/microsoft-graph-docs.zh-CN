---
title: managedAppFlaggedReason 枚举类型
description: 用户已被标记的原因
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 40a9d347a86df672f80ffe9b7aeda7f7f2750283
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43372929"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="185aa-103">managedAppFlaggedReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="185aa-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="185aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="185aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="185aa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="185aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="185aa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="185aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="185aa-107">用户已被标记的原因</span><span class="sxs-lookup"><span data-stu-id="185aa-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="185aa-108">成员</span><span class="sxs-lookup"><span data-stu-id="185aa-108">Members</span></span>
|<span data-ttu-id="185aa-109">成员</span><span class="sxs-lookup"><span data-stu-id="185aa-109">Member</span></span>|<span data-ttu-id="185aa-110">值</span><span class="sxs-lookup"><span data-stu-id="185aa-110">Value</span></span>|<span data-ttu-id="185aa-111">说明</span><span class="sxs-lookup"><span data-stu-id="185aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185aa-112">无</span><span class="sxs-lookup"><span data-stu-id="185aa-112">none</span></span>|<span data-ttu-id="185aa-113">0</span><span class="sxs-lookup"><span data-stu-id="185aa-113">0</span></span>|<span data-ttu-id="185aa-114">无问题。</span><span class="sxs-lookup"><span data-stu-id="185aa-114">No issue.</span></span>|
|<span data-ttu-id="185aa-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="185aa-115">rootedDevice</span></span>|<span data-ttu-id="185aa-116">1</span><span class="sxs-lookup"><span data-stu-id="185aa-116">1</span></span>|<span data-ttu-id="185aa-117">应用注册在根/解锁设备上运行。</span><span class="sxs-lookup"><span data-stu-id="185aa-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="185aa-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="185aa-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="185aa-119">双面</span><span class="sxs-lookup"><span data-stu-id="185aa-119">2</span></span>|<span data-ttu-id="185aa-120">应用注册在解锁了启用程序的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="185aa-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="185aa-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="185aa-121">androidFactoryRomModified</span></span>|<span data-ttu-id="185aa-122">第三章</span><span class="sxs-lookup"><span data-stu-id="185aa-122">3</span></span>|<span data-ttu-id="185aa-123">应用注册在已修改出厂 ROM 的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="185aa-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



