---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 08ac7a36e142a1d19dbaaeb0263ef095072a9e01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956813"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="7c67f-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7c67f-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="7c67f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7c67f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c67f-105">代表向其应用程序数据进行加密托管应用程序的级别</span><span class="sxs-lookup"><span data-stu-id="7c67f-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="7c67f-106">成员</span><span class="sxs-lookup"><span data-stu-id="7c67f-106">Members</span></span>
|<span data-ttu-id="7c67f-107">成员</span><span class="sxs-lookup"><span data-stu-id="7c67f-107">Member</span></span>|<span data-ttu-id="7c67f-108">值</span><span class="sxs-lookup"><span data-stu-id="7c67f-108">Value</span></span>|<span data-ttu-id="7c67f-109">Description</span><span class="sxs-lookup"><span data-stu-id="7c67f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c67f-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="7c67f-110">useDeviceSettings</span></span>|<span data-ttu-id="7c67f-111">0</span><span class="sxs-lookup"><span data-stu-id="7c67f-111">0</span></span>|<span data-ttu-id="7c67f-112">应用程序数据进行加密根据设备上的默认设置。</span><span class="sxs-lookup"><span data-stu-id="7c67f-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="7c67f-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="7c67f-113">afterDeviceRestart</span></span>|<span data-ttu-id="7c67f-114">1</span><span class="sxs-lookup"><span data-stu-id="7c67f-114">1</span></span>|<span data-ttu-id="7c67f-115">应用程序数据进行加密时重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="7c67f-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="7c67f-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="7c67f-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="7c67f-117">2</span><span class="sxs-lookup"><span data-stu-id="7c67f-117">2</span></span>|<span data-ttu-id="7c67f-118">与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据</span><span class="sxs-lookup"><span data-stu-id="7c67f-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="7c67f-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="7c67f-119">whenDeviceLocked</span></span>|<span data-ttu-id="7c67f-120">3</span><span class="sxs-lookup"><span data-stu-id="7c67f-120">3</span></span>|<span data-ttu-id="7c67f-121">与此策略关联的应用程序数据进行加密时设备锁定</span><span class="sxs-lookup"><span data-stu-id="7c67f-121">App data associated with this policy is encrypted when the device is locked</span></span>|



