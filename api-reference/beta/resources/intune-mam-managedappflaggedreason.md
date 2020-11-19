---
title: managedAppFlaggedReason 枚举类型
description: 用户已被标记的原因
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 08d21f78466f7f716b5d9bffcd1832e5c1a23d89
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259681"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="fd1b7-103">managedAppFlaggedReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fd1b7-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="fd1b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd1b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd1b7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd1b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd1b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd1b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd1b7-107">用户已被标记的原因</span><span class="sxs-lookup"><span data-stu-id="fd1b7-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="fd1b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="fd1b7-108">Members</span></span>
|<span data-ttu-id="fd1b7-109">成员</span><span class="sxs-lookup"><span data-stu-id="fd1b7-109">Member</span></span>|<span data-ttu-id="fd1b7-110">值</span><span class="sxs-lookup"><span data-stu-id="fd1b7-110">Value</span></span>|<span data-ttu-id="fd1b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd1b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd1b7-112">无</span><span class="sxs-lookup"><span data-stu-id="fd1b7-112">none</span></span>|<span data-ttu-id="fd1b7-113">0</span><span class="sxs-lookup"><span data-stu-id="fd1b7-113">0</span></span>|<span data-ttu-id="fd1b7-114">无问题。</span><span class="sxs-lookup"><span data-stu-id="fd1b7-114">No issue.</span></span>|
|<span data-ttu-id="fd1b7-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="fd1b7-115">rootedDevice</span></span>|<span data-ttu-id="fd1b7-116">1</span><span class="sxs-lookup"><span data-stu-id="fd1b7-116">1</span></span>|<span data-ttu-id="fd1b7-117">应用注册在根/解锁设备上运行。</span><span class="sxs-lookup"><span data-stu-id="fd1b7-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="fd1b7-118">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="fd1b7-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="fd1b7-119">双面</span><span class="sxs-lookup"><span data-stu-id="fd1b7-119">2</span></span>|<span data-ttu-id="fd1b7-120">应用注册在解锁了启用程序的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="fd1b7-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="fd1b7-121">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="fd1b7-121">androidFactoryRomModified</span></span>|<span data-ttu-id="fd1b7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fd1b7-122">3</span></span>|<span data-ttu-id="fd1b7-123">应用注册在已修改出厂 ROM 的 Android 设备上运行。</span><span class="sxs-lookup"><span data-stu-id="fd1b7-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|




