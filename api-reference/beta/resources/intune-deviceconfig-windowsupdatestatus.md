---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73cd3208b7729544d6fbd620a13ce295b39aff26
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780180"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="dc03f-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dc03f-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="dc03f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc03f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc03f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc03f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc03f-106">Windows update for business 配置设备状态</span><span class="sxs-lookup"><span data-stu-id="dc03f-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="dc03f-107">成员</span><span class="sxs-lookup"><span data-stu-id="dc03f-107">Members</span></span>
|<span data-ttu-id="dc03f-108">成员</span><span class="sxs-lookup"><span data-stu-id="dc03f-108">Member</span></span>|<span data-ttu-id="dc03f-109">值</span><span class="sxs-lookup"><span data-stu-id="dc03f-109">Value</span></span>|<span data-ttu-id="dc03f-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc03f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc03f-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="dc03f-111">upToDate</span></span>|<span data-ttu-id="dc03f-112">0</span><span class="sxs-lookup"><span data-stu-id="dc03f-112">0</span></span>|<span data-ttu-id="dc03f-113">没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="dc03f-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="dc03f-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="dc03f-114">pendingInstallation</span></span>|<span data-ttu-id="dc03f-115">1</span><span class="sxs-lookup"><span data-stu-id="dc03f-115">1</span></span>|<span data-ttu-id="dc03f-116">存在挂起安装的更新, 其中包括未批准的更新。</span><span class="sxs-lookup"><span data-stu-id="dc03f-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="dc03f-117">没有挂起的重新启动更新, 没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="dc03f-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="dc03f-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="dc03f-118">pendingReboot</span></span>|<span data-ttu-id="dc03f-119">双面</span><span class="sxs-lookup"><span data-stu-id="dc03f-119">2</span></span>|<span data-ttu-id="dc03f-120">存在需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="dc03f-120">There are updates that requires reboot.</span></span> <span data-ttu-id="dc03f-121">没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="dc03f-121">There are not failed updates.</span></span>|
|<span data-ttu-id="dc03f-122">未能</span><span class="sxs-lookup"><span data-stu-id="dc03f-122">failed</span></span>|<span data-ttu-id="dc03f-123">第三章</span><span class="sxs-lookup"><span data-stu-id="dc03f-123">3</span></span>|<span data-ttu-id="dc03f-124">无法在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="dc03f-124">There are updates failed to install on the device.</span></span>|





