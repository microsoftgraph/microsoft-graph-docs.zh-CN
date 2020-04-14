---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f854a18bfcfac3f937c976180bbc4a423abbae0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374035"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="ba35d-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ba35d-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="ba35d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba35d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba35d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba35d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba35d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba35d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba35d-107">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="ba35d-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="ba35d-108">成员</span><span class="sxs-lookup"><span data-stu-id="ba35d-108">Members</span></span>
|<span data-ttu-id="ba35d-109">成员</span><span class="sxs-lookup"><span data-stu-id="ba35d-109">Member</span></span>|<span data-ttu-id="ba35d-110">值</span><span class="sxs-lookup"><span data-stu-id="ba35d-110">Value</span></span>|<span data-ttu-id="ba35d-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba35d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba35d-112">allApps</span><span class="sxs-lookup"><span data-stu-id="ba35d-112">allApps</span></span>|<span data-ttu-id="ba35d-113">0</span><span class="sxs-lookup"><span data-stu-id="ba35d-113">0</span></span>|<span data-ttu-id="ba35d-114">允许在所有应用程序之间进行共享（托管或不允许）</span><span class="sxs-lookup"><span data-stu-id="ba35d-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="ba35d-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="ba35d-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="ba35d-116">1</span><span class="sxs-lookup"><span data-stu-id="ba35d-116">1</span></span>|<span data-ttu-id="ba35d-117">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="ba35d-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="ba35d-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="ba35d-118">managedApps</span></span>|<span data-ttu-id="ba35d-119">双面</span><span class="sxs-lookup"><span data-stu-id="ba35d-119">2</span></span>|<span data-ttu-id="ba35d-120">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="ba35d-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="ba35d-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="ba35d-121">blocked</span></span>|<span data-ttu-id="ba35d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ba35d-122">3</span></span>|<span data-ttu-id="ba35d-123">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="ba35d-123">Sharing between apps is disabled</span></span>|



