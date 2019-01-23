---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413687"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="5be6c-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5be6c-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="5be6c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5be6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5be6c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5be6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5be6c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5be6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5be6c-107">代表向其应用程序数据进行加密托管应用程序的级别</span><span class="sxs-lookup"><span data-stu-id="5be6c-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="5be6c-108">成员</span><span class="sxs-lookup"><span data-stu-id="5be6c-108">Members</span></span>
|<span data-ttu-id="5be6c-109">成员</span><span class="sxs-lookup"><span data-stu-id="5be6c-109">Member</span></span>|<span data-ttu-id="5be6c-110">值</span><span class="sxs-lookup"><span data-stu-id="5be6c-110">Value</span></span>|<span data-ttu-id="5be6c-111">说明</span><span class="sxs-lookup"><span data-stu-id="5be6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5be6c-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="5be6c-112">useDeviceSettings</span></span>|<span data-ttu-id="5be6c-113">0</span><span class="sxs-lookup"><span data-stu-id="5be6c-113">0</span></span>|<span data-ttu-id="5be6c-114">应用程序数据进行加密根据设备上的默认设置。</span><span class="sxs-lookup"><span data-stu-id="5be6c-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="5be6c-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="5be6c-115">afterDeviceRestart</span></span>|<span data-ttu-id="5be6c-116">1</span><span class="sxs-lookup"><span data-stu-id="5be6c-116">1</span></span>|<span data-ttu-id="5be6c-117">应用程序数据进行加密时重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="5be6c-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="5be6c-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="5be6c-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="5be6c-119">2</span><span class="sxs-lookup"><span data-stu-id="5be6c-119">2</span></span>|<span data-ttu-id="5be6c-120">与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据</span><span class="sxs-lookup"><span data-stu-id="5be6c-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="5be6c-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="5be6c-121">whenDeviceLocked</span></span>|<span data-ttu-id="5be6c-122">3</span><span class="sxs-lookup"><span data-stu-id="5be6c-122">3</span></span>|<span data-ttu-id="5be6c-123">与此策略关联的应用程序数据进行加密时设备锁定</span><span class="sxs-lookup"><span data-stu-id="5be6c-123">App data associated with this policy is encrypted when the device is locked</span></span>|




