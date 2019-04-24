---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465253"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="13450-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="13450-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="13450-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13450-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13450-105">表示为托管应用程序加密应用程序数据的级别</span><span class="sxs-lookup"><span data-stu-id="13450-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="13450-106">成员</span><span class="sxs-lookup"><span data-stu-id="13450-106">Members</span></span>
|<span data-ttu-id="13450-107">成员</span><span class="sxs-lookup"><span data-stu-id="13450-107">Member</span></span>|<span data-ttu-id="13450-108">值</span><span class="sxs-lookup"><span data-stu-id="13450-108">Value</span></span>|<span data-ttu-id="13450-109">说明</span><span class="sxs-lookup"><span data-stu-id="13450-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13450-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="13450-110">useDeviceSettings</span></span>|<span data-ttu-id="13450-111">0</span><span class="sxs-lookup"><span data-stu-id="13450-111">0</span></span>|<span data-ttu-id="13450-112">应用程序数据根据设备上的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="13450-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="13450-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="13450-113">afterDeviceRestart</span></span>|<span data-ttu-id="13450-114">1</span><span class="sxs-lookup"><span data-stu-id="13450-114">1</span></span>|<span data-ttu-id="13450-115">重新启动设备时对应用数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="13450-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="13450-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="13450-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="13450-117">2 </span><span class="sxs-lookup"><span data-stu-id="13450-117">2</span></span>|<span data-ttu-id="13450-118">设备锁定时, 与此策略关联的应用数据将被加密, 但打开的文件中的数据除外</span><span class="sxs-lookup"><span data-stu-id="13450-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="13450-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="13450-119">whenDeviceLocked</span></span>|<span data-ttu-id="13450-120">3 </span><span class="sxs-lookup"><span data-stu-id="13450-120">3</span></span>|<span data-ttu-id="13450-121">设备锁定时, 与此策略关联的应用数据将被加密</span><span class="sxs-lookup"><span data-stu-id="13450-121">App data associated with this policy is encrypted when the device is locked</span></span>|



