---
title: win32LobAppRestartBehavior 枚举类型
description: 指示重新启动操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc6ff030c2228ae108e034eea312c57d40b9006f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758965"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="9b74f-103">win32LobAppRestartBehavior 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b74f-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="9b74f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b74f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b74f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b74f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b74f-106">指示重新启动操作的类型。</span><span class="sxs-lookup"><span data-stu-id="9b74f-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="9b74f-107">成员</span><span class="sxs-lookup"><span data-stu-id="9b74f-107">Members</span></span>
|<span data-ttu-id="9b74f-108">成员</span><span class="sxs-lookup"><span data-stu-id="9b74f-108">Member</span></span>|<span data-ttu-id="9b74f-109">值</span><span class="sxs-lookup"><span data-stu-id="9b74f-109">Value</span></span>|<span data-ttu-id="9b74f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b74f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b74f-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="9b74f-111">basedOnReturnCode</span></span>|<span data-ttu-id="9b74f-112">0</span><span class="sxs-lookup"><span data-stu-id="9b74f-112">0</span></span>|<span data-ttu-id="9b74f-113">如果操作返回重启代码，Intune 将在运行应用安装后重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="9b74f-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="9b74f-114">allow</span><span class="sxs-lookup"><span data-stu-id="9b74f-114">allow</span></span>|<span data-ttu-id="9b74f-115">1</span><span class="sxs-lookup"><span data-stu-id="9b74f-115">1</span></span>|<span data-ttu-id="9b74f-116">Intune 不会对应用安装生成的重启代码执行任何特定操作。</span><span class="sxs-lookup"><span data-stu-id="9b74f-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="9b74f-117">Intune 不会尝试禁止为 MSI 应用重启。</span><span class="sxs-lookup"><span data-stu-id="9b74f-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="9b74f-118">suppress</span><span class="sxs-lookup"><span data-stu-id="9b74f-118">suppress</span></span>|<span data-ttu-id="9b74f-119">2</span><span class="sxs-lookup"><span data-stu-id="9b74f-119">2</span></span>|<span data-ttu-id="9b74f-120">Intune 将尝试禁止为 MSI 应用重启。</span><span class="sxs-lookup"><span data-stu-id="9b74f-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="9b74f-121">force</span><span class="sxs-lookup"><span data-stu-id="9b74f-121">force</span></span>|<span data-ttu-id="9b74f-122">3</span><span class="sxs-lookup"><span data-stu-id="9b74f-122">3</span></span>|<span data-ttu-id="9b74f-123">Intune 将强制设备在应用安装操作后立即重新启动。</span><span class="sxs-lookup"><span data-stu-id="9b74f-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|




