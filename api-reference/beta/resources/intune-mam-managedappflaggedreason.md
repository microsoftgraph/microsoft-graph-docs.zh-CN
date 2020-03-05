---
title: managedAppFlaggedReason 枚举类型
description: 用户已被标记的原因
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64f78ca8a074d35687f50e232a104b87717a6462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527919"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="f0275-103">managedAppFlaggedReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f0275-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="f0275-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0275-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0275-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0275-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0275-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0275-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0275-107">用户已被标记的原因</span><span class="sxs-lookup"><span data-stu-id="f0275-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="f0275-108">成员</span><span class="sxs-lookup"><span data-stu-id="f0275-108">Members</span></span>
|<span data-ttu-id="f0275-109">成员</span><span class="sxs-lookup"><span data-stu-id="f0275-109">Member</span></span>|<span data-ttu-id="f0275-110">值</span><span class="sxs-lookup"><span data-stu-id="f0275-110">Value</span></span>|<span data-ttu-id="f0275-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0275-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0275-112">无</span><span class="sxs-lookup"><span data-stu-id="f0275-112">none</span></span>|<span data-ttu-id="f0275-113">0</span><span class="sxs-lookup"><span data-stu-id="f0275-113">0</span></span>|<span data-ttu-id="f0275-114">无问题。</span><span class="sxs-lookup"><span data-stu-id="f0275-114">No issue.</span></span>|
|<span data-ttu-id="f0275-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="f0275-115">rootedDevice</span></span>|<span data-ttu-id="f0275-116">1 </span><span class="sxs-lookup"><span data-stu-id="f0275-116">1</span></span>|<span data-ttu-id="f0275-117">应用注册在根/解锁设备上运行。</span><span class="sxs-lookup"><span data-stu-id="f0275-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="f0275-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="f0275-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="f0275-119">2 </span><span class="sxs-lookup"><span data-stu-id="f0275-119">2</span></span>|<span data-ttu-id="f0275-120">应用注册在解锁了启用程序的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="f0275-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="f0275-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="f0275-121">androidFactoryRomModified</span></span>|<span data-ttu-id="f0275-122">3 </span><span class="sxs-lookup"><span data-stu-id="f0275-122">3</span></span>|<span data-ttu-id="f0275-123">应用注册在已修改出厂 ROM 的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="f0275-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



