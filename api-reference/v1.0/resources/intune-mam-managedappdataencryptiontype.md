---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b3e2cc44e1d548a1abe2a4d34c02fef9db7750a1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356385"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="48626-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="48626-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="48626-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48626-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48626-105">表示为托管应用程序加密应用程序数据的级别</span><span class="sxs-lookup"><span data-stu-id="48626-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="48626-106">成员</span><span class="sxs-lookup"><span data-stu-id="48626-106">Members</span></span>
|<span data-ttu-id="48626-107">成员</span><span class="sxs-lookup"><span data-stu-id="48626-107">Member</span></span>|<span data-ttu-id="48626-108">值</span><span class="sxs-lookup"><span data-stu-id="48626-108">Value</span></span>|<span data-ttu-id="48626-109">说明</span><span class="sxs-lookup"><span data-stu-id="48626-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48626-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="48626-110">useDeviceSettings</span></span>|<span data-ttu-id="48626-111">0</span><span class="sxs-lookup"><span data-stu-id="48626-111">0</span></span>|<span data-ttu-id="48626-112">应用程序数据根据设备上的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="48626-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="48626-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="48626-113">afterDeviceRestart</span></span>|<span data-ttu-id="48626-114">1</span><span class="sxs-lookup"><span data-stu-id="48626-114">1</span></span>|<span data-ttu-id="48626-115">重新启动设备时对应用数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="48626-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="48626-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="48626-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="48626-117">双面</span><span class="sxs-lookup"><span data-stu-id="48626-117">2</span></span>|<span data-ttu-id="48626-118">设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外</span><span class="sxs-lookup"><span data-stu-id="48626-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="48626-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="48626-119">whenDeviceLocked</span></span>|<span data-ttu-id="48626-120">第三章</span><span class="sxs-lookup"><span data-stu-id="48626-120">3</span></span>|<span data-ttu-id="48626-121">设备锁定时，与此策略关联的应用数据将被加密</span><span class="sxs-lookup"><span data-stu-id="48626-121">App data associated with this policy is encrypted when the device is locked</span></span>|




