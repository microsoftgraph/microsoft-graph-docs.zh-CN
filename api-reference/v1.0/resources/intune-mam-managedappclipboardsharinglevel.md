---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e16eb22dfe09135857eca5a936df4b276e465b2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356413"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="ba7e1-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ba7e1-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="ba7e1-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba7e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba7e1-105">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="ba7e1-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="ba7e1-106">成员</span><span class="sxs-lookup"><span data-stu-id="ba7e1-106">Members</span></span>
|<span data-ttu-id="ba7e1-107">成员</span><span class="sxs-lookup"><span data-stu-id="ba7e1-107">Member</span></span>|<span data-ttu-id="ba7e1-108">值</span><span class="sxs-lookup"><span data-stu-id="ba7e1-108">Value</span></span>|<span data-ttu-id="ba7e1-109">说明</span><span class="sxs-lookup"><span data-stu-id="ba7e1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba7e1-110">allApps</span><span class="sxs-lookup"><span data-stu-id="ba7e1-110">allApps</span></span>|<span data-ttu-id="ba7e1-111">0</span><span class="sxs-lookup"><span data-stu-id="ba7e1-111">0</span></span>|<span data-ttu-id="ba7e1-112">允许在所有应用程序之间进行共享（托管或不允许）</span><span class="sxs-lookup"><span data-stu-id="ba7e1-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="ba7e1-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="ba7e1-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="ba7e1-114">1</span><span class="sxs-lookup"><span data-stu-id="ba7e1-114">1</span></span>|<span data-ttu-id="ba7e1-115">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="ba7e1-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="ba7e1-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="ba7e1-116">managedApps</span></span>|<span data-ttu-id="ba7e1-117">双面</span><span class="sxs-lookup"><span data-stu-id="ba7e1-117">2</span></span>|<span data-ttu-id="ba7e1-118">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="ba7e1-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="ba7e1-119">堵塞</span><span class="sxs-lookup"><span data-stu-id="ba7e1-119">blocked</span></span>|<span data-ttu-id="ba7e1-120">第三章</span><span class="sxs-lookup"><span data-stu-id="ba7e1-120">3</span></span>|<span data-ttu-id="ba7e1-121">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="ba7e1-121">Sharing between apps is disabled</span></span>|




