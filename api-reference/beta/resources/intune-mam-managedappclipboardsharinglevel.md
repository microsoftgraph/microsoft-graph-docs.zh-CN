---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97e5e74b9d8f039e75df61791ef8dea945e49818
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527958"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="1d3eb-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1d3eb-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="1d3eb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1d3eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d3eb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d3eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d3eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d3eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d3eb-107">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="1d3eb-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="1d3eb-108">成员</span><span class="sxs-lookup"><span data-stu-id="1d3eb-108">Members</span></span>
|<span data-ttu-id="1d3eb-109">成员</span><span class="sxs-lookup"><span data-stu-id="1d3eb-109">Member</span></span>|<span data-ttu-id="1d3eb-110">值</span><span class="sxs-lookup"><span data-stu-id="1d3eb-110">Value</span></span>|<span data-ttu-id="1d3eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="1d3eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d3eb-112">allApps</span><span class="sxs-lookup"><span data-stu-id="1d3eb-112">allApps</span></span>|<span data-ttu-id="1d3eb-113">0</span><span class="sxs-lookup"><span data-stu-id="1d3eb-113">0</span></span>|<span data-ttu-id="1d3eb-114">允许在所有应用程序之间进行共享（托管或不允许）</span><span class="sxs-lookup"><span data-stu-id="1d3eb-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="1d3eb-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="1d3eb-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="1d3eb-116">1 </span><span class="sxs-lookup"><span data-stu-id="1d3eb-116">1</span></span>|<span data-ttu-id="1d3eb-117">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="1d3eb-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="1d3eb-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="1d3eb-118">managedApps</span></span>|<span data-ttu-id="1d3eb-119">2 </span><span class="sxs-lookup"><span data-stu-id="1d3eb-119">2</span></span>|<span data-ttu-id="1d3eb-120">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="1d3eb-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="1d3eb-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="1d3eb-121">blocked</span></span>|<span data-ttu-id="1d3eb-122">3 </span><span class="sxs-lookup"><span data-stu-id="1d3eb-122">3</span></span>|<span data-ttu-id="1d3eb-123">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="1d3eb-123">Sharing between apps is disabled</span></span>|



