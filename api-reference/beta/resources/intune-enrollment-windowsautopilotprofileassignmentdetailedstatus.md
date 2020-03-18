---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cc08aea928568e9d7c867e50706cfee34f34668c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783373"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="7df31-103">windowsAutopilotProfileAssignmentDetailedStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7df31-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

> <span data-ttu-id="7df31-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7df31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7df31-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7df31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df31-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7df31-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="7df31-107">成员</span><span class="sxs-lookup"><span data-stu-id="7df31-107">Members</span></span>
|<span data-ttu-id="7df31-108">成员</span><span class="sxs-lookup"><span data-stu-id="7df31-108">Member</span></span>|<span data-ttu-id="7df31-109">值</span><span class="sxs-lookup"><span data-stu-id="7df31-109">Value</span></span>|<span data-ttu-id="7df31-110">说明</span><span class="sxs-lookup"><span data-stu-id="7df31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df31-111">无</span><span class="sxs-lookup"><span data-stu-id="7df31-111">none</span></span>|<span data-ttu-id="7df31-112">0</span><span class="sxs-lookup"><span data-stu-id="7df31-112">0</span></span>|<span data-ttu-id="7df31-113">无分配详细状态</span><span class="sxs-lookup"><span data-stu-id="7df31-113">No assignment detailed status</span></span>|
|<span data-ttu-id="7df31-114">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="7df31-114">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="7df31-115">1</span><span class="sxs-lookup"><span data-stu-id="7df31-115">1</span></span>|<span data-ttu-id="7df31-116">不满足硬件要求。</span><span class="sxs-lookup"><span data-stu-id="7df31-116">Hardware requirements are not met.</span></span> <span data-ttu-id="7df31-117">如果将自部署 AutoPilot 配置文件分配给不安装 TPM 2.0 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7df31-117">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="7df31-118">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="7df31-118">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="7df31-119">双面</span><span class="sxs-lookup"><span data-stu-id="7df31-119">2</span></span>|<span data-ttu-id="7df31-120">如果 SurfaceHub AutoPilot 配置文件分配给不是 SurfaceHub 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7df31-120">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="7df31-121">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="7df31-121">holoLensProfileNotSupported</span></span>|<span data-ttu-id="7df31-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7df31-122">3</span></span>|<span data-ttu-id="7df31-123">如果将 HoloLens AutoPilot 配置文件分配给非 HoloLens 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7df31-123">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="7df31-124">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="7df31-124">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="7df31-125">4 </span><span class="sxs-lookup"><span data-stu-id="7df31-125">4</span></span>|<span data-ttu-id="7df31-126">如果 WindowsPc AutoPilot 配置文件分配给不是 WindowsPc 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7df31-126">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



