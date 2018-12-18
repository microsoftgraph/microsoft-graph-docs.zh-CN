---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
author: tfitzmac
ms.openlocfilehash: 6bd23f6cd590724c2c981ddf2c3087ead4c21817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326115"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="390ec-103">managedAppDataEncryptionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="390ec-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="390ec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="390ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="390ec-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="390ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="390ec-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="390ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="390ec-107">代表向其应用程序数据进行加密托管应用程序的级别</span><span class="sxs-lookup"><span data-stu-id="390ec-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="390ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="390ec-108">Members</span></span>
|<span data-ttu-id="390ec-109">成员</span><span class="sxs-lookup"><span data-stu-id="390ec-109">Member</span></span>|<span data-ttu-id="390ec-110">值</span><span class="sxs-lookup"><span data-stu-id="390ec-110">Value</span></span>|<span data-ttu-id="390ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="390ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="390ec-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="390ec-112">useDeviceSettings</span></span>|<span data-ttu-id="390ec-113">0</span><span class="sxs-lookup"><span data-stu-id="390ec-113">0</span></span>|<span data-ttu-id="390ec-114">应用程序数据进行加密根据设备上的默认设置。</span><span class="sxs-lookup"><span data-stu-id="390ec-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="390ec-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="390ec-115">afterDeviceRestart</span></span>|<span data-ttu-id="390ec-116">1</span><span class="sxs-lookup"><span data-stu-id="390ec-116">1</span></span>|<span data-ttu-id="390ec-117">应用程序数据进行加密时重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="390ec-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="390ec-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="390ec-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="390ec-119">2</span><span class="sxs-lookup"><span data-stu-id="390ec-119">2</span></span>|<span data-ttu-id="390ec-120">与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据</span><span class="sxs-lookup"><span data-stu-id="390ec-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="390ec-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="390ec-121">whenDeviceLocked</span></span>|<span data-ttu-id="390ec-122">3</span><span class="sxs-lookup"><span data-stu-id="390ec-122">3</span></span>|<span data-ttu-id="390ec-123">与此策略关联的应用程序数据进行加密时设备锁定</span><span class="sxs-lookup"><span data-stu-id="390ec-123">App data associated with this policy is encrypted when the device is locked</span></span>|





