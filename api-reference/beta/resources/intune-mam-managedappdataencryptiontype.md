---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 962e759e83b08baf7fc150e07dc84ed7146feb0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563852"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="c16b4-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c16b4-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="c16b4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c16b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c16b4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c16b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c16b4-106">表示为托管应用程序加密应用程序数据的级别</span><span class="sxs-lookup"><span data-stu-id="c16b4-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="c16b4-107">成员</span><span class="sxs-lookup"><span data-stu-id="c16b4-107">Members</span></span>
|<span data-ttu-id="c16b4-108">成员</span><span class="sxs-lookup"><span data-stu-id="c16b4-108">Member</span></span>|<span data-ttu-id="c16b4-109">值</span><span class="sxs-lookup"><span data-stu-id="c16b4-109">Value</span></span>|<span data-ttu-id="c16b4-110">说明</span><span class="sxs-lookup"><span data-stu-id="c16b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c16b4-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="c16b4-111">useDeviceSettings</span></span>|<span data-ttu-id="c16b4-112">0</span><span class="sxs-lookup"><span data-stu-id="c16b4-112">0</span></span>|<span data-ttu-id="c16b4-113">应用程序数据根据设备上的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="c16b4-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="c16b4-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="c16b4-114">afterDeviceRestart</span></span>|<span data-ttu-id="c16b4-115">1</span><span class="sxs-lookup"><span data-stu-id="c16b4-115">1</span></span>|<span data-ttu-id="c16b4-116">重新启动设备时对应用数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="c16b4-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="c16b4-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="c16b4-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="c16b4-118">2 </span><span class="sxs-lookup"><span data-stu-id="c16b4-118">2</span></span>|<span data-ttu-id="c16b4-119">设备锁定时, 与此策略关联的应用数据将被加密, 但打开的文件中的数据除外</span><span class="sxs-lookup"><span data-stu-id="c16b4-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="c16b4-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="c16b4-120">whenDeviceLocked</span></span>|<span data-ttu-id="c16b4-121">3 </span><span class="sxs-lookup"><span data-stu-id="c16b4-121">3</span></span>|<span data-ttu-id="c16b4-122">设备锁定时, 与此策略关联的应用数据将被加密</span><span class="sxs-lookup"><span data-stu-id="c16b4-122">App data associated with this policy is encrypted when the device is locked</span></span>|





