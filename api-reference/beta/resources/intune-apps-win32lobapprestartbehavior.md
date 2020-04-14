---
title: win32LobAppRestartBehavior 枚举类型
description: 指示重新启动操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2902f3808ea1ebcc1442b0675c89da51b059f2c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422637"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="d63e2-103">win32LobAppRestartBehavior 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d63e2-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="d63e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d63e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d63e2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d63e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d63e2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d63e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d63e2-107">指示重新启动操作的类型。</span><span class="sxs-lookup"><span data-stu-id="d63e2-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="d63e2-108">成员</span><span class="sxs-lookup"><span data-stu-id="d63e2-108">Members</span></span>
|<span data-ttu-id="d63e2-109">成员</span><span class="sxs-lookup"><span data-stu-id="d63e2-109">Member</span></span>|<span data-ttu-id="d63e2-110">值</span><span class="sxs-lookup"><span data-stu-id="d63e2-110">Value</span></span>|<span data-ttu-id="d63e2-111">说明</span><span class="sxs-lookup"><span data-stu-id="d63e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d63e2-112">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="d63e2-112">basedOnReturnCode</span></span>|<span data-ttu-id="d63e2-113">0</span><span class="sxs-lookup"><span data-stu-id="d63e2-113">0</span></span>|<span data-ttu-id="d63e2-114">如果操作返回重新启动代码，则在运行应用程序安装后，Intune 将重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="d63e2-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="d63e2-115">允许</span><span class="sxs-lookup"><span data-stu-id="d63e2-115">allow</span></span>|<span data-ttu-id="d63e2-116">1</span><span class="sxs-lookup"><span data-stu-id="d63e2-116">1</span></span>|<span data-ttu-id="d63e2-117">Intune 不会对由应用安装引起的重新启动代码执行任何特定操作。</span><span class="sxs-lookup"><span data-stu-id="d63e2-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="d63e2-118">Intune 不会尝试取消对 MSI 应用的重新启动。</span><span class="sxs-lookup"><span data-stu-id="d63e2-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="d63e2-119">强制</span><span class="sxs-lookup"><span data-stu-id="d63e2-119">suppress</span></span>|<span data-ttu-id="d63e2-120">双面</span><span class="sxs-lookup"><span data-stu-id="d63e2-120">2</span></span>|<span data-ttu-id="d63e2-121">Intune 将尝试取消对 MSI 应用的重新启动。</span><span class="sxs-lookup"><span data-stu-id="d63e2-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="d63e2-122">有效</span><span class="sxs-lookup"><span data-stu-id="d63e2-122">force</span></span>|<span data-ttu-id="d63e2-123">第三章</span><span class="sxs-lookup"><span data-stu-id="d63e2-123">3</span></span>|<span data-ttu-id="d63e2-124">Intune 将强制在应用程序安装操作完成后立即重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="d63e2-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|



