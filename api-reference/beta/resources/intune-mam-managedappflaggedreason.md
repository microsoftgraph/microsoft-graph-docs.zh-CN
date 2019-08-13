---
title: managedAppFlaggedReason 枚举类型
description: 用户已被标记的原因
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7aedda5d89d41ba936651c10d81ceeb33dfe603a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332124"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="fca57-103">managedAppFlaggedReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fca57-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="fca57-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fca57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fca57-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fca57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fca57-106">用户已被标记的原因</span><span class="sxs-lookup"><span data-stu-id="fca57-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="fca57-107">成员</span><span class="sxs-lookup"><span data-stu-id="fca57-107">Members</span></span>
|<span data-ttu-id="fca57-108">成员</span><span class="sxs-lookup"><span data-stu-id="fca57-108">Member</span></span>|<span data-ttu-id="fca57-109">值</span><span class="sxs-lookup"><span data-stu-id="fca57-109">Value</span></span>|<span data-ttu-id="fca57-110">说明</span><span class="sxs-lookup"><span data-stu-id="fca57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fca57-111">无</span><span class="sxs-lookup"><span data-stu-id="fca57-111">none</span></span>|<span data-ttu-id="fca57-112">0</span><span class="sxs-lookup"><span data-stu-id="fca57-112">0</span></span>|<span data-ttu-id="fca57-113">无问题。</span><span class="sxs-lookup"><span data-stu-id="fca57-113">No issue.</span></span>|
|<span data-ttu-id="fca57-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="fca57-114">rootedDevice</span></span>|<span data-ttu-id="fca57-115">1</span><span class="sxs-lookup"><span data-stu-id="fca57-115">1</span></span>|<span data-ttu-id="fca57-116">应用注册在根/解锁设备上运行。</span><span class="sxs-lookup"><span data-stu-id="fca57-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="fca57-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="fca57-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="fca57-118">双面</span><span class="sxs-lookup"><span data-stu-id="fca57-118">2</span></span>|<span data-ttu-id="fca57-119">应用注册在解锁了启用程序的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="fca57-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="fca57-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="fca57-120">androidFactoryRomModified</span></span>|<span data-ttu-id="fca57-121">第三章</span><span class="sxs-lookup"><span data-stu-id="fca57-121">3</span></span>|<span data-ttu-id="fca57-122">应用注册在已修改出厂 ROM 的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="fca57-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



