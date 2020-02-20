---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 418670dd5f334b169d43022a9908c2a39f279b60
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163897"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="7693e-103">windowsAutopilotProfileAssignmentDetailedStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7693e-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

> <span data-ttu-id="7693e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7693e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7693e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7693e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7693e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7693e-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="7693e-107">成员</span><span class="sxs-lookup"><span data-stu-id="7693e-107">Members</span></span>
|<span data-ttu-id="7693e-108">成员</span><span class="sxs-lookup"><span data-stu-id="7693e-108">Member</span></span>|<span data-ttu-id="7693e-109">值</span><span class="sxs-lookup"><span data-stu-id="7693e-109">Value</span></span>|<span data-ttu-id="7693e-110">说明</span><span class="sxs-lookup"><span data-stu-id="7693e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7693e-111">无</span><span class="sxs-lookup"><span data-stu-id="7693e-111">none</span></span>|<span data-ttu-id="7693e-112">0</span><span class="sxs-lookup"><span data-stu-id="7693e-112">0</span></span>|<span data-ttu-id="7693e-113">无分配详细状态</span><span class="sxs-lookup"><span data-stu-id="7693e-113">No assignment detailed status</span></span>|
|<span data-ttu-id="7693e-114">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="7693e-114">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="7693e-115">1</span><span class="sxs-lookup"><span data-stu-id="7693e-115">1</span></span>|<span data-ttu-id="7693e-116">不满足硬件要求。</span><span class="sxs-lookup"><span data-stu-id="7693e-116">Hardware requirements are not met.</span></span> <span data-ttu-id="7693e-117">如果将自部署 AutoPilot 配置文件分配给不安装 TPM 2.0 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7693e-117">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="7693e-118">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="7693e-118">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="7693e-119">双面</span><span class="sxs-lookup"><span data-stu-id="7693e-119">2</span></span>|<span data-ttu-id="7693e-120">如果 SurfaceHub AutoPilot 配置文件分配给不是 SurfaceHub 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7693e-120">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="7693e-121">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="7693e-121">holoLensProfileNotSupported</span></span>|<span data-ttu-id="7693e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7693e-122">3</span></span>|<span data-ttu-id="7693e-123">如果将 HoloLens AutoPilot 配置文件分配给非 HoloLens 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7693e-123">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="7693e-124">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="7693e-124">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="7693e-125">4</span><span class="sxs-lookup"><span data-stu-id="7693e-125">4</span></span>|<span data-ttu-id="7693e-126">如果 WindowsPc AutoPilot 配置文件分配给不是 WindowsPc 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="7693e-126">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



