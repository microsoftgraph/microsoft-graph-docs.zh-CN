---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15ae82a4eef55b67a08e53a191c5ffebc9ae2c6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030428"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="9eee1-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9eee1-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="9eee1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eee1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9eee1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9eee1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9eee1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9eee1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eee1-107">表示为托管应用程序加密应用程序数据的级别</span><span class="sxs-lookup"><span data-stu-id="9eee1-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="9eee1-108">成员</span><span class="sxs-lookup"><span data-stu-id="9eee1-108">Members</span></span>
|<span data-ttu-id="9eee1-109">成员</span><span class="sxs-lookup"><span data-stu-id="9eee1-109">Member</span></span>|<span data-ttu-id="9eee1-110">值</span><span class="sxs-lookup"><span data-stu-id="9eee1-110">Value</span></span>|<span data-ttu-id="9eee1-111">说明</span><span class="sxs-lookup"><span data-stu-id="9eee1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eee1-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="9eee1-112">useDeviceSettings</span></span>|<span data-ttu-id="9eee1-113">0</span><span class="sxs-lookup"><span data-stu-id="9eee1-113">0</span></span>|<span data-ttu-id="9eee1-114">应用程序数据根据设备上的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="9eee1-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="9eee1-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="9eee1-115">afterDeviceRestart</span></span>|<span data-ttu-id="9eee1-116">1 </span><span class="sxs-lookup"><span data-stu-id="9eee1-116">1</span></span>|<span data-ttu-id="9eee1-117">重新启动设备时对应用数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="9eee1-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="9eee1-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="9eee1-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="9eee1-119">2 </span><span class="sxs-lookup"><span data-stu-id="9eee1-119">2</span></span>|<span data-ttu-id="9eee1-120">设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外</span><span class="sxs-lookup"><span data-stu-id="9eee1-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="9eee1-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="9eee1-121">whenDeviceLocked</span></span>|<span data-ttu-id="9eee1-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9eee1-122">3</span></span>|<span data-ttu-id="9eee1-123">设备锁定时，与此策略关联的应用数据将被加密</span><span class="sxs-lookup"><span data-stu-id="9eee1-123">App data associated with this policy is encrypted when the device is locked</span></span>|






