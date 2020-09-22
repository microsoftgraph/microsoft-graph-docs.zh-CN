---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3567bc5262bb30612c3b4b9389f28435c3d623d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031590"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="2d4ab-103">windowsAutopilotProfileAssignmentDetailedStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2d4ab-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

<span data-ttu-id="2d4ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d4ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d4ab-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d4ab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d4ab-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2d4ab-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="2d4ab-108">成员</span><span class="sxs-lookup"><span data-stu-id="2d4ab-108">Members</span></span>
|<span data-ttu-id="2d4ab-109">成员</span><span class="sxs-lookup"><span data-stu-id="2d4ab-109">Member</span></span>|<span data-ttu-id="2d4ab-110">值</span><span class="sxs-lookup"><span data-stu-id="2d4ab-110">Value</span></span>|<span data-ttu-id="2d4ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="2d4ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d4ab-112">无</span><span class="sxs-lookup"><span data-stu-id="2d4ab-112">none</span></span>|<span data-ttu-id="2d4ab-113">0</span><span class="sxs-lookup"><span data-stu-id="2d4ab-113">0</span></span>|<span data-ttu-id="2d4ab-114">无分配详细状态</span><span class="sxs-lookup"><span data-stu-id="2d4ab-114">No assignment detailed status</span></span>|
|<span data-ttu-id="2d4ab-115">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="2d4ab-115">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="2d4ab-116">1 </span><span class="sxs-lookup"><span data-stu-id="2d4ab-116">1</span></span>|<span data-ttu-id="2d4ab-117">不满足硬件要求。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-117">Hardware requirements are not met.</span></span> <span data-ttu-id="2d4ab-118">如果将自部署 AutoPilot 配置文件分配给不安装 TPM 2.0 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-118">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="2d4ab-119">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="2d4ab-119">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="2d4ab-120">2 </span><span class="sxs-lookup"><span data-stu-id="2d4ab-120">2</span></span>|<span data-ttu-id="2d4ab-121">如果 SurfaceHub AutoPilot 配置文件分配给不是 SurfaceHub 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-121">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="2d4ab-122">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="2d4ab-122">holoLensProfileNotSupported</span></span>|<span data-ttu-id="2d4ab-123">第三章</span><span class="sxs-lookup"><span data-stu-id="2d4ab-123">3</span></span>|<span data-ttu-id="2d4ab-124">如果将 HoloLens AutoPilot 配置文件分配给非 HoloLens 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-124">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="2d4ab-125">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="2d4ab-125">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="2d4ab-126">4 </span><span class="sxs-lookup"><span data-stu-id="2d4ab-126">4</span></span>|<span data-ttu-id="2d4ab-127">如果 WindowsPc AutoPilot 配置文件分配给不是 WindowsPc 的设备，则可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="2d4ab-127">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|






