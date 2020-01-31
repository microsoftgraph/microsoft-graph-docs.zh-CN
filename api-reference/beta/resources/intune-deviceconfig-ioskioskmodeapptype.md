---
title: iosKioskModeAppType 枚举类型
description: IOS 展台模式的应用程序源选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bc92978d9d5f54395d8580598008a4bb3140666d
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636684"
---
# <a name="ioskioskmodeapptype-enum-type"></a><span data-ttu-id="0cc6d-103">iosKioskModeAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0cc6d-103">iosKioskModeAppType enum type</span></span>

> <span data-ttu-id="0cc6d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cc6d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cc6d-106">IOS 展台模式的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-106">App source options for iOS kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="0cc6d-107">成员</span><span class="sxs-lookup"><span data-stu-id="0cc6d-107">Members</span></span>
|<span data-ttu-id="0cc6d-108">成员</span><span class="sxs-lookup"><span data-stu-id="0cc6d-108">Member</span></span>|<span data-ttu-id="0cc6d-109">值</span><span class="sxs-lookup"><span data-stu-id="0cc6d-109">Value</span></span>|<span data-ttu-id="0cc6d-110">Description</span><span class="sxs-lookup"><span data-stu-id="0cc6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc6d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0cc6d-111">notConfigured</span></span>|<span data-ttu-id="0cc6d-112">0</span><span class="sxs-lookup"><span data-stu-id="0cc6d-112">0</span></span>|<span data-ttu-id="0cc6d-113">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="0cc6d-114">appStoreApp</span><span class="sxs-lookup"><span data-stu-id="0cc6d-114">appStoreApp</span></span>|<span data-ttu-id="0cc6d-115">1 </span><span class="sxs-lookup"><span data-stu-id="0cc6d-115">1</span></span>|<span data-ttu-id="0cc6d-116">要运行的应用程序来自应用商店。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-116">The app to be run comes from the app store.</span></span>|
|<span data-ttu-id="0cc6d-117">managedApp</span><span class="sxs-lookup"><span data-stu-id="0cc6d-117">managedApp</span></span>|<span data-ttu-id="0cc6d-118">2 </span><span class="sxs-lookup"><span data-stu-id="0cc6d-118">2</span></span>|<span data-ttu-id="0cc6d-119">要运行的应用程序内置于设备中。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-119">The app to be run is built into the device.</span></span>|
|<span data-ttu-id="0cc6d-120">builtInApp</span><span class="sxs-lookup"><span data-stu-id="0cc6d-120">builtInApp</span></span>|<span data-ttu-id="0cc6d-121">3 </span><span class="sxs-lookup"><span data-stu-id="0cc6d-121">3</span></span>|<span data-ttu-id="0cc6d-122">要运行的应用程序是托管应用程序。</span><span class="sxs-lookup"><span data-stu-id="0cc6d-122">The app to be run is a managed app.</span></span>|



