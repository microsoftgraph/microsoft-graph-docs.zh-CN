---
title: iosKioskModeAppType 枚举类型
description: IOS 展台模式的应用程序源选项。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db614c90612e940405bb7ca13908e5efef419d70
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440285"
---
# <a name="ioskioskmodeapptype-enum-type"></a><span data-ttu-id="33458-103">iosKioskModeAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="33458-103">iosKioskModeAppType enum type</span></span>

<span data-ttu-id="33458-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33458-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33458-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33458-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33458-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33458-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33458-107">IOS 展台模式的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="33458-107">App source options for iOS kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="33458-108">成员</span><span class="sxs-lookup"><span data-stu-id="33458-108">Members</span></span>
|<span data-ttu-id="33458-109">成员</span><span class="sxs-lookup"><span data-stu-id="33458-109">Member</span></span>|<span data-ttu-id="33458-110">值</span><span class="sxs-lookup"><span data-stu-id="33458-110">Value</span></span>|<span data-ttu-id="33458-111">说明</span><span class="sxs-lookup"><span data-stu-id="33458-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33458-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="33458-112">notConfigured</span></span>|<span data-ttu-id="33458-113">0</span><span class="sxs-lookup"><span data-stu-id="33458-113">0</span></span>|<span data-ttu-id="33458-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="33458-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="33458-115">appStoreApp</span><span class="sxs-lookup"><span data-stu-id="33458-115">appStoreApp</span></span>|<span data-ttu-id="33458-116">1</span><span class="sxs-lookup"><span data-stu-id="33458-116">1</span></span>|<span data-ttu-id="33458-117">要运行的应用程序来自应用商店。</span><span class="sxs-lookup"><span data-stu-id="33458-117">The app to be run comes from the app store.</span></span>|
|<span data-ttu-id="33458-118">managedApp</span><span class="sxs-lookup"><span data-stu-id="33458-118">managedApp</span></span>|<span data-ttu-id="33458-119">双面</span><span class="sxs-lookup"><span data-stu-id="33458-119">2</span></span>|<span data-ttu-id="33458-120">要运行的应用程序内置于设备中。</span><span class="sxs-lookup"><span data-stu-id="33458-120">The app to be run is built into the device.</span></span>|
|<span data-ttu-id="33458-121">builtInApp</span><span class="sxs-lookup"><span data-stu-id="33458-121">builtInApp</span></span>|<span data-ttu-id="33458-122">第三章</span><span class="sxs-lookup"><span data-stu-id="33458-122">3</span></span>|<span data-ttu-id="33458-123">要运行的应用程序是托管应用程序。</span><span class="sxs-lookup"><span data-stu-id="33458-123">The app to be run is a managed app.</span></span>|



