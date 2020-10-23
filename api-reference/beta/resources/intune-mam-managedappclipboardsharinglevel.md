---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7daab906ab376aea8b7540b88c6922a37ec23bd2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684643"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="c319e-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c319e-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="c319e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c319e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c319e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c319e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c319e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c319e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c319e-107">表示可在应用程序之间共享设备的剪贴板的级别</span><span class="sxs-lookup"><span data-stu-id="c319e-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="c319e-108">成员</span><span class="sxs-lookup"><span data-stu-id="c319e-108">Members</span></span>
|<span data-ttu-id="c319e-109">成员</span><span class="sxs-lookup"><span data-stu-id="c319e-109">Member</span></span>|<span data-ttu-id="c319e-110">值</span><span class="sxs-lookup"><span data-stu-id="c319e-110">Value</span></span>|<span data-ttu-id="c319e-111">说明</span><span class="sxs-lookup"><span data-stu-id="c319e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c319e-112">allApps</span><span class="sxs-lookup"><span data-stu-id="c319e-112">allApps</span></span>|<span data-ttu-id="c319e-113">0</span><span class="sxs-lookup"><span data-stu-id="c319e-113">0</span></span>|<span data-ttu-id="c319e-114">允许在所有应用程序之间进行共享（托管或不允许）</span><span class="sxs-lookup"><span data-stu-id="c319e-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="c319e-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="c319e-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="c319e-116">1</span><span class="sxs-lookup"><span data-stu-id="c319e-116">1</span></span>|<span data-ttu-id="c319e-117">允许在启用了粘贴的所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="c319e-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="c319e-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="c319e-118">managedApps</span></span>|<span data-ttu-id="c319e-119">双面</span><span class="sxs-lookup"><span data-stu-id="c319e-119">2</span></span>|<span data-ttu-id="c319e-120">允许在所有托管应用之间进行共享</span><span class="sxs-lookup"><span data-stu-id="c319e-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="c319e-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="c319e-121">blocked</span></span>|<span data-ttu-id="c319e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c319e-122">3</span></span>|<span data-ttu-id="c319e-123">已禁用应用程序之间的共享</span><span class="sxs-lookup"><span data-stu-id="c319e-123">Sharing between apps is disabled</span></span>|





