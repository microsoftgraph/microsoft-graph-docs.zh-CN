---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c78ab8cbe35bdef9317069aac9612f14ba2a2e2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524572"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="a4b81-103">windowsAutopilotProfileAssignmentDetailedStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a4b81-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

<span data-ttu-id="a4b81-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a4b81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4b81-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4b81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4b81-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4b81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4b81-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a4b81-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="a4b81-108">成员</span><span class="sxs-lookup"><span data-stu-id="a4b81-108">Members</span></span>
|<span data-ttu-id="a4b81-109">成员</span><span class="sxs-lookup"><span data-stu-id="a4b81-109">Member</span></span>|<span data-ttu-id="a4b81-110">值</span><span class="sxs-lookup"><span data-stu-id="a4b81-110">Value</span></span>|<span data-ttu-id="a4b81-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4b81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4b81-112">无</span><span class="sxs-lookup"><span data-stu-id="a4b81-112">none</span></span>|<span data-ttu-id="a4b81-113">0</span><span class="sxs-lookup"><span data-stu-id="a4b81-113">0</span></span>|<span data-ttu-id="a4b81-114">无分配详细状态</span><span class="sxs-lookup"><span data-stu-id="a4b81-114">No assignment detailed status</span></span>|
|<span data-ttu-id="a4b81-115">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="a4b81-115">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="a4b81-116">1 </span><span class="sxs-lookup"><span data-stu-id="a4b81-116">1</span></span>|<span data-ttu-id="a4b81-117">不满足硬件要求。</span><span class="sxs-lookup"><span data-stu-id="a4b81-117">Hardware requirements are not met.</span></span> <span data-ttu-id="a4b81-118">如果将自部署 AutoPilot 配置文件分配给不安装 TPM 2.0 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="a4b81-118">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="a4b81-119">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="a4b81-119">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="a4b81-120">2 </span><span class="sxs-lookup"><span data-stu-id="a4b81-120">2</span></span>|<span data-ttu-id="a4b81-121">如果 SurfaceHub AutoPilot 配置文件分配给不是 SurfaceHub 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="a4b81-121">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="a4b81-122">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="a4b81-122">holoLensProfileNotSupported</span></span>|<span data-ttu-id="a4b81-123">3 </span><span class="sxs-lookup"><span data-stu-id="a4b81-123">3</span></span>|<span data-ttu-id="a4b81-124">如果将 HoloLens AutoPilot 配置文件分配给非 HoloLens 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="a4b81-124">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="a4b81-125">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="a4b81-125">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="a4b81-126">4 </span><span class="sxs-lookup"><span data-stu-id="a4b81-126">4</span></span>|<span data-ttu-id="a4b81-127">如果 WindowsPc AutoPilot 配置文件分配给不是 WindowsPc 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="a4b81-127">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



