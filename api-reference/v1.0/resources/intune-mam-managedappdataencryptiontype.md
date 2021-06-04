---
title: managedAppDataEncryptionType 枚举类型
description: 表示对托管应用加密的应用数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a3cbe74f8dbc81330b899b4acedcbc880b8d81d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754495"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="36eec-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="36eec-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="36eec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36eec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36eec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36eec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36eec-106">表示对托管应用加密的应用数据的级别</span><span class="sxs-lookup"><span data-stu-id="36eec-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="36eec-107">成员</span><span class="sxs-lookup"><span data-stu-id="36eec-107">Members</span></span>
|<span data-ttu-id="36eec-108">成员</span><span class="sxs-lookup"><span data-stu-id="36eec-108">Member</span></span>|<span data-ttu-id="36eec-109">值</span><span class="sxs-lookup"><span data-stu-id="36eec-109">Value</span></span>|<span data-ttu-id="36eec-110">Description</span><span class="sxs-lookup"><span data-stu-id="36eec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36eec-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="36eec-111">useDeviceSettings</span></span>|<span data-ttu-id="36eec-112">0</span><span class="sxs-lookup"><span data-stu-id="36eec-112">0</span></span>|<span data-ttu-id="36eec-113">应用数据根据设备的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="36eec-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="36eec-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="36eec-114">afterDeviceRestart</span></span>|<span data-ttu-id="36eec-115">1</span><span class="sxs-lookup"><span data-stu-id="36eec-115">1</span></span>|<span data-ttu-id="36eec-116">应用数据在设备重启时加密。</span><span class="sxs-lookup"><span data-stu-id="36eec-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="36eec-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="36eec-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="36eec-118">2</span><span class="sxs-lookup"><span data-stu-id="36eec-118">2</span></span>|<span data-ttu-id="36eec-119">与此策略关联的应用数据在设备锁定时加密，打开的文件的数据除外</span><span class="sxs-lookup"><span data-stu-id="36eec-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="36eec-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="36eec-120">whenDeviceLocked</span></span>|<span data-ttu-id="36eec-121">3</span><span class="sxs-lookup"><span data-stu-id="36eec-121">3</span></span>|<span data-ttu-id="36eec-122">与此策略关联的应用数据在设备锁定时加密</span><span class="sxs-lookup"><span data-stu-id="36eec-122">App data associated with this policy is encrypted when the device is locked</span></span>|




