---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5f6153eeb4b76af9d8974b715b7c6342c646ba6e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782242"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="79410-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="79410-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="79410-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79410-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79410-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79410-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79410-106">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="79410-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="79410-107">成员</span><span class="sxs-lookup"><span data-stu-id="79410-107">Members</span></span>
|<span data-ttu-id="79410-108">成员</span><span class="sxs-lookup"><span data-stu-id="79410-108">Member</span></span>|<span data-ttu-id="79410-109">值</span><span class="sxs-lookup"><span data-stu-id="79410-109">Value</span></span>|<span data-ttu-id="79410-110">说明</span><span class="sxs-lookup"><span data-stu-id="79410-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79410-111">allApps</span><span class="sxs-lookup"><span data-stu-id="79410-111">allApps</span></span>|<span data-ttu-id="79410-112">0</span><span class="sxs-lookup"><span data-stu-id="79410-112">0</span></span>|<span data-ttu-id="79410-113">允许在所有应用程序之间进行共享（托管或不允许）</span><span class="sxs-lookup"><span data-stu-id="79410-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="79410-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="79410-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="79410-115">1</span><span class="sxs-lookup"><span data-stu-id="79410-115">1</span></span>|<span data-ttu-id="79410-116">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="79410-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="79410-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="79410-117">managedApps</span></span>|<span data-ttu-id="79410-118">双面</span><span class="sxs-lookup"><span data-stu-id="79410-118">2</span></span>|<span data-ttu-id="79410-119">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="79410-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="79410-120">堵塞</span><span class="sxs-lookup"><span data-stu-id="79410-120">blocked</span></span>|<span data-ttu-id="79410-121">第三章</span><span class="sxs-lookup"><span data-stu-id="79410-121">3</span></span>|<span data-ttu-id="79410-122">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="79410-122">Sharing between apps is disabled</span></span>|



