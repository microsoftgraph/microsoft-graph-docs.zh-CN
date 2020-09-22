---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 140593618ed781d6033ea36deed481a6601b3352
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039628"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="6a35e-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6a35e-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="6a35e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a35e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a35e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a35e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a35e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a35e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a35e-107">Windows update for business 配置设备状态</span><span class="sxs-lookup"><span data-stu-id="6a35e-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="6a35e-108">成员</span><span class="sxs-lookup"><span data-stu-id="6a35e-108">Members</span></span>
|<span data-ttu-id="6a35e-109">成员</span><span class="sxs-lookup"><span data-stu-id="6a35e-109">Member</span></span>|<span data-ttu-id="6a35e-110">值</span><span class="sxs-lookup"><span data-stu-id="6a35e-110">Value</span></span>|<span data-ttu-id="6a35e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6a35e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a35e-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="6a35e-112">upToDate</span></span>|<span data-ttu-id="6a35e-113">0</span><span class="sxs-lookup"><span data-stu-id="6a35e-113">0</span></span>|<span data-ttu-id="6a35e-114">没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="6a35e-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="6a35e-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="6a35e-115">pendingInstallation</span></span>|<span data-ttu-id="6a35e-116">1 </span><span class="sxs-lookup"><span data-stu-id="6a35e-116">1</span></span>|<span data-ttu-id="6a35e-117">存在挂起安装的更新，其中包括未批准的更新。</span><span class="sxs-lookup"><span data-stu-id="6a35e-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="6a35e-118">没有挂起的重新启动更新，没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="6a35e-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="6a35e-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="6a35e-119">pendingReboot</span></span>|<span data-ttu-id="6a35e-120">2 </span><span class="sxs-lookup"><span data-stu-id="6a35e-120">2</span></span>|<span data-ttu-id="6a35e-121">存在需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="6a35e-121">There are updates that requires reboot.</span></span> <span data-ttu-id="6a35e-122">没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="6a35e-122">There are not failed updates.</span></span>|
|<span data-ttu-id="6a35e-123">未能</span><span class="sxs-lookup"><span data-stu-id="6a35e-123">failed</span></span>|<span data-ttu-id="6a35e-124">第三章</span><span class="sxs-lookup"><span data-stu-id="6a35e-124">3</span></span>|<span data-ttu-id="6a35e-125">无法在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="6a35e-125">There are updates failed to install on the device.</span></span>|






