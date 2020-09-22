---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e02d2dd993a31056a19d4c54155b1195e93ab58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074956"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="4ce57-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4ce57-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="4ce57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ce57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ce57-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ce57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ce57-106">表示为托管应用程序加密应用程序数据的级别</span><span class="sxs-lookup"><span data-stu-id="4ce57-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="4ce57-107">成员</span><span class="sxs-lookup"><span data-stu-id="4ce57-107">Members</span></span>
|<span data-ttu-id="4ce57-108">成员</span><span class="sxs-lookup"><span data-stu-id="4ce57-108">Member</span></span>|<span data-ttu-id="4ce57-109">值</span><span class="sxs-lookup"><span data-stu-id="4ce57-109">Value</span></span>|<span data-ttu-id="4ce57-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ce57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ce57-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="4ce57-111">useDeviceSettings</span></span>|<span data-ttu-id="4ce57-112">0</span><span class="sxs-lookup"><span data-stu-id="4ce57-112">0</span></span>|<span data-ttu-id="4ce57-113">应用程序数据根据设备上的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="4ce57-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="4ce57-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="4ce57-114">afterDeviceRestart</span></span>|<span data-ttu-id="4ce57-115">1 </span><span class="sxs-lookup"><span data-stu-id="4ce57-115">1</span></span>|<span data-ttu-id="4ce57-116">重新启动设备时对应用数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="4ce57-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="4ce57-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="4ce57-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="4ce57-118">2 </span><span class="sxs-lookup"><span data-stu-id="4ce57-118">2</span></span>|<span data-ttu-id="4ce57-119">设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外</span><span class="sxs-lookup"><span data-stu-id="4ce57-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="4ce57-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="4ce57-120">whenDeviceLocked</span></span>|<span data-ttu-id="4ce57-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4ce57-121">3</span></span>|<span data-ttu-id="4ce57-122">设备锁定时，与此策略关联的应用数据将被加密</span><span class="sxs-lookup"><span data-stu-id="4ce57-122">App data associated with this policy is encrypted when the device is locked</span></span>|









