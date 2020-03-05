---
title: iosKioskModeAppType 枚举类型
description: IOS 展台模式的应用程序源选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03e5d1c20f64a816160e2d9fa4292388d49bb50b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529888"
---
# <a name="ioskioskmodeapptype-enum-type"></a><span data-ttu-id="e1a8a-103">iosKioskModeAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1a8a-103">iosKioskModeAppType enum type</span></span>

<span data-ttu-id="e1a8a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e1a8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1a8a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1a8a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a8a-107">IOS 展台模式的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-107">App source options for iOS kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="e1a8a-108">成员</span><span class="sxs-lookup"><span data-stu-id="e1a8a-108">Members</span></span>
|<span data-ttu-id="e1a8a-109">成员</span><span class="sxs-lookup"><span data-stu-id="e1a8a-109">Member</span></span>|<span data-ttu-id="e1a8a-110">值</span><span class="sxs-lookup"><span data-stu-id="e1a8a-110">Value</span></span>|<span data-ttu-id="e1a8a-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1a8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a8a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e1a8a-112">notConfigured</span></span>|<span data-ttu-id="e1a8a-113">0</span><span class="sxs-lookup"><span data-stu-id="e1a8a-113">0</span></span>|<span data-ttu-id="e1a8a-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e1a8a-115">appStoreApp</span><span class="sxs-lookup"><span data-stu-id="e1a8a-115">appStoreApp</span></span>|<span data-ttu-id="e1a8a-116">1 </span><span class="sxs-lookup"><span data-stu-id="e1a8a-116">1</span></span>|<span data-ttu-id="e1a8a-117">要运行的应用程序来自应用商店。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-117">The app to be run comes from the app store.</span></span>|
|<span data-ttu-id="e1a8a-118">managedApp</span><span class="sxs-lookup"><span data-stu-id="e1a8a-118">managedApp</span></span>|<span data-ttu-id="e1a8a-119">2 </span><span class="sxs-lookup"><span data-stu-id="e1a8a-119">2</span></span>|<span data-ttu-id="e1a8a-120">要运行的应用程序内置于设备中。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-120">The app to be run is built into the device.</span></span>|
|<span data-ttu-id="e1a8a-121">builtInApp</span><span class="sxs-lookup"><span data-stu-id="e1a8a-121">builtInApp</span></span>|<span data-ttu-id="e1a8a-122">3 </span><span class="sxs-lookup"><span data-stu-id="e1a8a-122">3</span></span>|<span data-ttu-id="e1a8a-123">要运行的应用程序是托管应用程序。</span><span class="sxs-lookup"><span data-stu-id="e1a8a-123">The app to be run is a managed app.</span></span>|



