---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0151a572011f9033ae7b622e5d3cf2bfd086ed39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706931"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="106b5-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="106b5-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="106b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="106b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="106b5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="106b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="106b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="106b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="106b5-107">Windows update for business 配置设备状态</span><span class="sxs-lookup"><span data-stu-id="106b5-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="106b5-108">成员</span><span class="sxs-lookup"><span data-stu-id="106b5-108">Members</span></span>
|<span data-ttu-id="106b5-109">成员</span><span class="sxs-lookup"><span data-stu-id="106b5-109">Member</span></span>|<span data-ttu-id="106b5-110">值</span><span class="sxs-lookup"><span data-stu-id="106b5-110">Value</span></span>|<span data-ttu-id="106b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="106b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="106b5-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="106b5-112">upToDate</span></span>|<span data-ttu-id="106b5-113">0</span><span class="sxs-lookup"><span data-stu-id="106b5-113">0</span></span>|<span data-ttu-id="106b5-114">没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="106b5-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="106b5-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="106b5-115">pendingInstallation</span></span>|<span data-ttu-id="106b5-116">1</span><span class="sxs-lookup"><span data-stu-id="106b5-116">1</span></span>|<span data-ttu-id="106b5-117">存在挂起安装的更新，其中包括未批准的更新。</span><span class="sxs-lookup"><span data-stu-id="106b5-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="106b5-118">没有挂起的重新启动更新，没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="106b5-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="106b5-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="106b5-119">pendingReboot</span></span>|<span data-ttu-id="106b5-120">双面</span><span class="sxs-lookup"><span data-stu-id="106b5-120">2</span></span>|<span data-ttu-id="106b5-121">存在需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="106b5-121">There are updates that requires reboot.</span></span> <span data-ttu-id="106b5-122">没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="106b5-122">There are not failed updates.</span></span>|
|<span data-ttu-id="106b5-123">未能</span><span class="sxs-lookup"><span data-stu-id="106b5-123">failed</span></span>|<span data-ttu-id="106b5-124">第三章</span><span class="sxs-lookup"><span data-stu-id="106b5-124">3</span></span>|<span data-ttu-id="106b5-125">无法在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="106b5-125">There are updates failed to install on the device.</span></span>|





