---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a09aca9ce1ac4cd81e09b8db8da10ea563f1f03
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272365"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="6d611-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6d611-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="6d611-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d611-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d611-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d611-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d611-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d611-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d611-107">Windows update for business 配置设备状态</span><span class="sxs-lookup"><span data-stu-id="6d611-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="6d611-108">成员</span><span class="sxs-lookup"><span data-stu-id="6d611-108">Members</span></span>
|<span data-ttu-id="6d611-109">成员</span><span class="sxs-lookup"><span data-stu-id="6d611-109">Member</span></span>|<span data-ttu-id="6d611-110">值</span><span class="sxs-lookup"><span data-stu-id="6d611-110">Value</span></span>|<span data-ttu-id="6d611-111">说明</span><span class="sxs-lookup"><span data-stu-id="6d611-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d611-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="6d611-112">upToDate</span></span>|<span data-ttu-id="6d611-113">0</span><span class="sxs-lookup"><span data-stu-id="6d611-113">0</span></span>|<span data-ttu-id="6d611-114">没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="6d611-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="6d611-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="6d611-115">pendingInstallation</span></span>|<span data-ttu-id="6d611-116">1</span><span class="sxs-lookup"><span data-stu-id="6d611-116">1</span></span>|<span data-ttu-id="6d611-117">存在挂起安装的更新，其中包括未批准的更新。</span><span class="sxs-lookup"><span data-stu-id="6d611-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="6d611-118">没有挂起的重新启动更新，没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="6d611-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="6d611-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="6d611-119">pendingReboot</span></span>|<span data-ttu-id="6d611-120">双面</span><span class="sxs-lookup"><span data-stu-id="6d611-120">2</span></span>|<span data-ttu-id="6d611-121">存在需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="6d611-121">There are updates that requires reboot.</span></span> <span data-ttu-id="6d611-122">没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="6d611-122">There are not failed updates.</span></span>|
|<span data-ttu-id="6d611-123">未能</span><span class="sxs-lookup"><span data-stu-id="6d611-123">failed</span></span>|<span data-ttu-id="6d611-124">第三章</span><span class="sxs-lookup"><span data-stu-id="6d611-124">3</span></span>|<span data-ttu-id="6d611-125">无法在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="6d611-125">There are updates failed to install on the device.</span></span>|




