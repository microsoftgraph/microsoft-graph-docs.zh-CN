---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7549fb77cf5a9f7c3014192d5524019323405f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154157"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="5b19a-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5b19a-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="5b19a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5b19a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b19a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b19a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b19a-106">Windows update for business 配置设备状态</span><span class="sxs-lookup"><span data-stu-id="5b19a-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="5b19a-107">成员</span><span class="sxs-lookup"><span data-stu-id="5b19a-107">Members</span></span>
|<span data-ttu-id="5b19a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5b19a-108">Member</span></span>|<span data-ttu-id="5b19a-109">值</span><span class="sxs-lookup"><span data-stu-id="5b19a-109">Value</span></span>|<span data-ttu-id="5b19a-110">说明</span><span class="sxs-lookup"><span data-stu-id="5b19a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b19a-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="5b19a-111">upToDate</span></span>|<span data-ttu-id="5b19a-112">0</span><span class="sxs-lookup"><span data-stu-id="5b19a-112">0</span></span>|<span data-ttu-id="5b19a-113">没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="5b19a-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="5b19a-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="5b19a-114">pendingInstallation</span></span>|<span data-ttu-id="5b19a-115">1</span><span class="sxs-lookup"><span data-stu-id="5b19a-115">1</span></span>|<span data-ttu-id="5b19a-116">存在挂起安装的更新, 其中包括未批准的更新。</span><span class="sxs-lookup"><span data-stu-id="5b19a-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="5b19a-117">没有挂起的重新启动更新, 没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="5b19a-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="5b19a-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="5b19a-118">pendingReboot</span></span>|<span data-ttu-id="5b19a-119">双面</span><span class="sxs-lookup"><span data-stu-id="5b19a-119">2</span></span>|<span data-ttu-id="5b19a-120">存在需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="5b19a-120">There are updates that requires reboot.</span></span> <span data-ttu-id="5b19a-121">没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="5b19a-121">There are not failed updates.</span></span>|
|<span data-ttu-id="5b19a-122">failed</span><span class="sxs-lookup"><span data-stu-id="5b19a-122">failed</span></span>|<span data-ttu-id="5b19a-123">第三章</span><span class="sxs-lookup"><span data-stu-id="5b19a-123">3</span></span>|<span data-ttu-id="5b19a-124">无法在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="5b19a-124">There are updates failed to install on the device.</span></span>|




