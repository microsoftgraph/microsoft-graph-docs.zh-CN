---
title: windowsUpdateStatus 枚举类型
description: Windows update for business 配置设备状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ce9ae47680408f50ef5ce42606cd856ac13ddc1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199897"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="98cb8-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="98cb8-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="98cb8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98cb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98cb8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98cb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98cb8-106">Windows update for business 配置设备状态</span><span class="sxs-lookup"><span data-stu-id="98cb8-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="98cb8-107">成员</span><span class="sxs-lookup"><span data-stu-id="98cb8-107">Members</span></span>
|<span data-ttu-id="98cb8-108">成员</span><span class="sxs-lookup"><span data-stu-id="98cb8-108">Member</span></span>|<span data-ttu-id="98cb8-109">值</span><span class="sxs-lookup"><span data-stu-id="98cb8-109">Value</span></span>|<span data-ttu-id="98cb8-110">说明</span><span class="sxs-lookup"><span data-stu-id="98cb8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98cb8-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="98cb8-111">upToDate</span></span>|<span data-ttu-id="98cb8-112">0</span><span class="sxs-lookup"><span data-stu-id="98cb8-112">0</span></span>|<span data-ttu-id="98cb8-113">没有挂起的更新、没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="98cb8-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="98cb8-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="98cb8-114">pendingInstallation</span></span>|<span data-ttu-id="98cb8-115">1</span><span class="sxs-lookup"><span data-stu-id="98cb8-115">1</span></span>|<span data-ttu-id="98cb8-116">存在挂起安装的更新，其中包括未批准的更新。</span><span class="sxs-lookup"><span data-stu-id="98cb8-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="98cb8-117">没有挂起的重新启动更新，没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="98cb8-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="98cb8-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="98cb8-118">pendingReboot</span></span>|<span data-ttu-id="98cb8-119">双面</span><span class="sxs-lookup"><span data-stu-id="98cb8-119">2</span></span>|<span data-ttu-id="98cb8-120">存在需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="98cb8-120">There are updates that requires reboot.</span></span> <span data-ttu-id="98cb8-121">没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="98cb8-121">There are not failed updates.</span></span>|
|<span data-ttu-id="98cb8-122">未能</span><span class="sxs-lookup"><span data-stu-id="98cb8-122">failed</span></span>|<span data-ttu-id="98cb8-123">第三章</span><span class="sxs-lookup"><span data-stu-id="98cb8-123">3</span></span>|<span data-ttu-id="98cb8-124">无法在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="98cb8-124">There are updates failed to install on the device.</span></span>|



