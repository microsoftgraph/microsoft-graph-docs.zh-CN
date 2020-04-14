---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f735a5ce77c0162899d7e93974a07de4f0be137b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469161"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="9b528-103">dmaGuardDeviceEnumerationPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b528-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="9b528-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b528-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b528-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b528-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b528-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b528-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b528-107">DmaGuardDeviceEnumerationPolicy 的可能值。</span><span class="sxs-lookup"><span data-stu-id="9b528-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="9b528-108">成员</span><span class="sxs-lookup"><span data-stu-id="9b528-108">Members</span></span>
|<span data-ttu-id="9b528-109">成员</span><span class="sxs-lookup"><span data-stu-id="9b528-109">Member</span></span>|<span data-ttu-id="9b528-110">值</span><span class="sxs-lookup"><span data-stu-id="9b528-110">Value</span></span>|<span data-ttu-id="9b528-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b528-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b528-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9b528-112">deviceDefault</span></span>|<span data-ttu-id="9b528-113">0</span><span class="sxs-lookup"><span data-stu-id="9b528-113">0</span></span>|<span data-ttu-id="9b528-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="9b528-114">Default value.</span></span> <span data-ttu-id="9b528-115">具有 DMA 重新映射的设备将仅在用户解锁屏幕后枚举不兼容驱动程序。</span><span class="sxs-lookup"><span data-stu-id="9b528-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="9b528-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="9b528-116">blockAll</span></span>|<span data-ttu-id="9b528-117">1</span><span class="sxs-lookup"><span data-stu-id="9b528-117">1</span></span>|<span data-ttu-id="9b528-118">具有 DMA 重新映射的设备不支持的驱动程序在任何时候都不能随时启动和执行 DMA。</span><span class="sxs-lookup"><span data-stu-id="9b528-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="9b528-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="9b528-119">allowAll</span></span>|<span data-ttu-id="9b528-120">双面</span><span class="sxs-lookup"><span data-stu-id="9b528-120">2</span></span>|<span data-ttu-id="9b528-121">所有支持外部 DMA 的 PCIe 设备将在任何时候枚举。</span><span class="sxs-lookup"><span data-stu-id="9b528-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



