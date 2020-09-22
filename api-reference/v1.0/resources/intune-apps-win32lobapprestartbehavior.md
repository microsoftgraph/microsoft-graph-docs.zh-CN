---
title: win32LobAppRestartBehavior 枚举类型
description: 指示重新启动操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a4f9044e90c67afe3ec50ba2349a94d194641dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036709"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="a2d8d-103">win32LobAppRestartBehavior 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a2d8d-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="a2d8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2d8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2d8d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2d8d-106">指示重新启动操作的类型。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="a2d8d-107">成员</span><span class="sxs-lookup"><span data-stu-id="a2d8d-107">Members</span></span>
|<span data-ttu-id="a2d8d-108">成员</span><span class="sxs-lookup"><span data-stu-id="a2d8d-108">Member</span></span>|<span data-ttu-id="a2d8d-109">值</span><span class="sxs-lookup"><span data-stu-id="a2d8d-109">Value</span></span>|<span data-ttu-id="a2d8d-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2d8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2d8d-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="a2d8d-111">basedOnReturnCode</span></span>|<span data-ttu-id="a2d8d-112">0</span><span class="sxs-lookup"><span data-stu-id="a2d8d-112">0</span></span>|<span data-ttu-id="a2d8d-113">如果操作返回重新启动代码，则在运行应用程序安装后，Intune 将重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="a2d8d-114">允许</span><span class="sxs-lookup"><span data-stu-id="a2d8d-114">allow</span></span>|<span data-ttu-id="a2d8d-115">1 </span><span class="sxs-lookup"><span data-stu-id="a2d8d-115">1</span></span>|<span data-ttu-id="a2d8d-116">Intune 不会对由应用安装引起的重新启动代码执行任何特定操作。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="a2d8d-117">Intune 不会尝试取消对 MSI 应用的重新启动。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="a2d8d-118">强制</span><span class="sxs-lookup"><span data-stu-id="a2d8d-118">suppress</span></span>|<span data-ttu-id="a2d8d-119">2 </span><span class="sxs-lookup"><span data-stu-id="a2d8d-119">2</span></span>|<span data-ttu-id="a2d8d-120">Intune 将尝试取消对 MSI 应用的重新启动。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="a2d8d-121">有效</span><span class="sxs-lookup"><span data-stu-id="a2d8d-121">force</span></span>|<span data-ttu-id="a2d8d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="a2d8d-122">3</span></span>|<span data-ttu-id="a2d8d-123">Intune 将强制在应用程序安装操作完成后立即重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="a2d8d-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|





