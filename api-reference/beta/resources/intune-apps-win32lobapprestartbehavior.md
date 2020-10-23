---
title: win32LobAppRestartBehavior 枚举类型
description: 指示重新启动操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4ce16d0c064fb182352fa0a0061fb2296fd44d7a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706182"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="b1852-103">win32LobAppRestartBehavior 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1852-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="b1852-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1852-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1852-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1852-107">指示重新启动操作的类型。</span><span class="sxs-lookup"><span data-stu-id="b1852-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="b1852-108">成员</span><span class="sxs-lookup"><span data-stu-id="b1852-108">Members</span></span>
|<span data-ttu-id="b1852-109">成员</span><span class="sxs-lookup"><span data-stu-id="b1852-109">Member</span></span>|<span data-ttu-id="b1852-110">值</span><span class="sxs-lookup"><span data-stu-id="b1852-110">Value</span></span>|<span data-ttu-id="b1852-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1852-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1852-112">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="b1852-112">basedOnReturnCode</span></span>|<span data-ttu-id="b1852-113">0</span><span class="sxs-lookup"><span data-stu-id="b1852-113">0</span></span>|<span data-ttu-id="b1852-114">如果操作返回重新启动代码，则在运行应用程序安装后，Intune 将重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="b1852-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="b1852-115">允许</span><span class="sxs-lookup"><span data-stu-id="b1852-115">allow</span></span>|<span data-ttu-id="b1852-116">1</span><span class="sxs-lookup"><span data-stu-id="b1852-116">1</span></span>|<span data-ttu-id="b1852-117">Intune 不会对由应用安装引起的重新启动代码执行任何特定操作。</span><span class="sxs-lookup"><span data-stu-id="b1852-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="b1852-118">Intune 不会尝试取消对 MSI 应用的重新启动。</span><span class="sxs-lookup"><span data-stu-id="b1852-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="b1852-119">强制</span><span class="sxs-lookup"><span data-stu-id="b1852-119">suppress</span></span>|<span data-ttu-id="b1852-120">双面</span><span class="sxs-lookup"><span data-stu-id="b1852-120">2</span></span>|<span data-ttu-id="b1852-121">Intune 将尝试取消对 MSI 应用的重新启动。</span><span class="sxs-lookup"><span data-stu-id="b1852-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="b1852-122">有效</span><span class="sxs-lookup"><span data-stu-id="b1852-122">force</span></span>|<span data-ttu-id="b1852-123">第三章</span><span class="sxs-lookup"><span data-stu-id="b1852-123">3</span></span>|<span data-ttu-id="b1852-124">Intune 将强制在应用程序安装操作完成后立即重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="b1852-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|





