---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
author: tfitzmac
ms.openlocfilehash: 3cbb733eb578ca839e32851d8a6d217f69d6799d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330322"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="08ee1-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="08ee1-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="08ee1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="08ee1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08ee1-105">代表向其应用程序数据进行加密托管应用程序的级别</span><span class="sxs-lookup"><span data-stu-id="08ee1-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="08ee1-106">成员</span><span class="sxs-lookup"><span data-stu-id="08ee1-106">Members</span></span>
|<span data-ttu-id="08ee1-107">成员</span><span class="sxs-lookup"><span data-stu-id="08ee1-107">Member</span></span>|<span data-ttu-id="08ee1-108">值</span><span class="sxs-lookup"><span data-stu-id="08ee1-108">Value</span></span>|<span data-ttu-id="08ee1-109">说明</span><span class="sxs-lookup"><span data-stu-id="08ee1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ee1-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="08ee1-110">useDeviceSettings</span></span>|<span data-ttu-id="08ee1-111">0</span><span class="sxs-lookup"><span data-stu-id="08ee1-111">0</span></span>|<span data-ttu-id="08ee1-112">应用程序数据进行加密根据设备上的默认设置。</span><span class="sxs-lookup"><span data-stu-id="08ee1-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="08ee1-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="08ee1-113">afterDeviceRestart</span></span>|<span data-ttu-id="08ee1-114">1</span><span class="sxs-lookup"><span data-stu-id="08ee1-114">1</span></span>|<span data-ttu-id="08ee1-115">应用程序数据进行加密时重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="08ee1-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="08ee1-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="08ee1-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="08ee1-117">2</span><span class="sxs-lookup"><span data-stu-id="08ee1-117">2</span></span>|<span data-ttu-id="08ee1-118">与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据</span><span class="sxs-lookup"><span data-stu-id="08ee1-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="08ee1-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="08ee1-119">whenDeviceLocked</span></span>|<span data-ttu-id="08ee1-120">3</span><span class="sxs-lookup"><span data-stu-id="08ee1-120">3</span></span>|<span data-ttu-id="08ee1-121">与此策略关联的应用程序数据进行加密时设备锁定</span><span class="sxs-lookup"><span data-stu-id="08ee1-121">App data associated with this policy is encrypted when the device is locked</span></span>|



