---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1bc52b0fa05a65adfb3e195d0a38c9bebd78e6c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267031"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="9812a-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9812a-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="9812a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9812a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9812a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9812a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9812a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9812a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9812a-107">表示为托管应用程序加密应用程序数据的级别</span><span class="sxs-lookup"><span data-stu-id="9812a-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="9812a-108">成员</span><span class="sxs-lookup"><span data-stu-id="9812a-108">Members</span></span>
|<span data-ttu-id="9812a-109">成员</span><span class="sxs-lookup"><span data-stu-id="9812a-109">Member</span></span>|<span data-ttu-id="9812a-110">值</span><span class="sxs-lookup"><span data-stu-id="9812a-110">Value</span></span>|<span data-ttu-id="9812a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9812a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9812a-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="9812a-112">useDeviceSettings</span></span>|<span data-ttu-id="9812a-113">0</span><span class="sxs-lookup"><span data-stu-id="9812a-113">0</span></span>|<span data-ttu-id="9812a-114">应用程序数据根据设备上的默认设置进行加密。</span><span class="sxs-lookup"><span data-stu-id="9812a-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="9812a-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="9812a-115">afterDeviceRestart</span></span>|<span data-ttu-id="9812a-116">1</span><span class="sxs-lookup"><span data-stu-id="9812a-116">1</span></span>|<span data-ttu-id="9812a-117">重新启动设备时对应用数据进行加密。</span><span class="sxs-lookup"><span data-stu-id="9812a-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="9812a-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="9812a-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="9812a-119">双面</span><span class="sxs-lookup"><span data-stu-id="9812a-119">2</span></span>|<span data-ttu-id="9812a-120">设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外</span><span class="sxs-lookup"><span data-stu-id="9812a-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="9812a-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="9812a-121">whenDeviceLocked</span></span>|<span data-ttu-id="9812a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9812a-122">3</span></span>|<span data-ttu-id="9812a-123">设备锁定时，与此策略关联的应用数据将被加密</span><span class="sxs-lookup"><span data-stu-id="9812a-123">App data associated with this policy is encrypted when the device is locked</span></span>|




