---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55a9608144e31d9e11f1a435e9220934ee3cb792
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445820"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="2b7ff-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2b7ff-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="2b7ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b7ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b7ff-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b7ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7ff-106">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="2b7ff-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="2b7ff-107">成员</span><span class="sxs-lookup"><span data-stu-id="2b7ff-107">Members</span></span>
|<span data-ttu-id="2b7ff-108">成员</span><span class="sxs-lookup"><span data-stu-id="2b7ff-108">Member</span></span>|<span data-ttu-id="2b7ff-109">值</span><span class="sxs-lookup"><span data-stu-id="2b7ff-109">Value</span></span>|<span data-ttu-id="2b7ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="2b7ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b7ff-111">allApps</span><span class="sxs-lookup"><span data-stu-id="2b7ff-111">allApps</span></span>|<span data-ttu-id="2b7ff-112">0</span><span class="sxs-lookup"><span data-stu-id="2b7ff-112">0</span></span>|<span data-ttu-id="2b7ff-113">允许在所有应用程序之间进行共享（托管或不允许）</span><span class="sxs-lookup"><span data-stu-id="2b7ff-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="2b7ff-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="2b7ff-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="2b7ff-115">1</span><span class="sxs-lookup"><span data-stu-id="2b7ff-115">1</span></span>|<span data-ttu-id="2b7ff-116">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="2b7ff-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="2b7ff-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="2b7ff-117">managedApps</span></span>|<span data-ttu-id="2b7ff-118">双面</span><span class="sxs-lookup"><span data-stu-id="2b7ff-118">2</span></span>|<span data-ttu-id="2b7ff-119">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="2b7ff-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="2b7ff-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="2b7ff-120">blocked</span></span>|<span data-ttu-id="2b7ff-121">第三章</span><span class="sxs-lookup"><span data-stu-id="2b7ff-121">3</span></span>|<span data-ttu-id="2b7ff-122">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="2b7ff-122">Sharing between apps is disabled</span></span>|







