---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465200"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="2f956-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2f956-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="2f956-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f956-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f956-105">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="2f956-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="2f956-106">成员</span><span class="sxs-lookup"><span data-stu-id="2f956-106">Members</span></span>
|<span data-ttu-id="2f956-107">成员</span><span class="sxs-lookup"><span data-stu-id="2f956-107">Member</span></span>|<span data-ttu-id="2f956-108">值</span><span class="sxs-lookup"><span data-stu-id="2f956-108">Value</span></span>|<span data-ttu-id="2f956-109">说明</span><span class="sxs-lookup"><span data-stu-id="2f956-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f956-110">allApps</span><span class="sxs-lookup"><span data-stu-id="2f956-110">allApps</span></span>|<span data-ttu-id="2f956-111">0</span><span class="sxs-lookup"><span data-stu-id="2f956-111">0</span></span>|<span data-ttu-id="2f956-112">允许在所有应用程序之间进行共享 (托管或不允许)</span><span class="sxs-lookup"><span data-stu-id="2f956-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="2f956-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="2f956-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="2f956-114">1</span><span class="sxs-lookup"><span data-stu-id="2f956-114">1</span></span>|<span data-ttu-id="2f956-115">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="2f956-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="2f956-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="2f956-116">managedApps</span></span>|<span data-ttu-id="2f956-117">2 </span><span class="sxs-lookup"><span data-stu-id="2f956-117">2</span></span>|<span data-ttu-id="2f956-118">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="2f956-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="2f956-119">堵塞</span><span class="sxs-lookup"><span data-stu-id="2f956-119">blocked</span></span>|<span data-ttu-id="2f956-120">3 </span><span class="sxs-lookup"><span data-stu-id="2f956-120">3</span></span>|<span data-ttu-id="2f956-121">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="2f956-121">Sharing between apps is disabled</span></span>|



