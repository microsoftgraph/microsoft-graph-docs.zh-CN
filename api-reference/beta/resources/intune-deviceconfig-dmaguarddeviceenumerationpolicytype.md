---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03e93e6ad3e5dae8a455bb3ceb9aa65f11dcf2e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526576"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="d6c5a-103">dmaGuardDeviceEnumerationPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d6c5a-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="d6c5a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d6c5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6c5a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6c5a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c5a-107">DmaGuardDeviceEnumerationPolicy 的可能值。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="d6c5a-108">成员</span><span class="sxs-lookup"><span data-stu-id="d6c5a-108">Members</span></span>
|<span data-ttu-id="d6c5a-109">成员</span><span class="sxs-lookup"><span data-stu-id="d6c5a-109">Member</span></span>|<span data-ttu-id="d6c5a-110">值</span><span class="sxs-lookup"><span data-stu-id="d6c5a-110">Value</span></span>|<span data-ttu-id="d6c5a-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6c5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c5a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d6c5a-112">deviceDefault</span></span>|<span data-ttu-id="d6c5a-113">0</span><span class="sxs-lookup"><span data-stu-id="d6c5a-113">0</span></span>|<span data-ttu-id="d6c5a-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-114">Default value.</span></span> <span data-ttu-id="d6c5a-115">具有 DMA 重新映射的设备将仅在用户解锁屏幕后枚举不兼容驱动程序。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="d6c5a-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="d6c5a-116">blockAll</span></span>|<span data-ttu-id="d6c5a-117">1 </span><span class="sxs-lookup"><span data-stu-id="d6c5a-117">1</span></span>|<span data-ttu-id="d6c5a-118">具有 DMA 重新映射的设备不支持的驱动程序在任何时候都不能随时启动和执行 DMA。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="d6c5a-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="d6c5a-119">allowAll</span></span>|<span data-ttu-id="d6c5a-120">2 </span><span class="sxs-lookup"><span data-stu-id="d6c5a-120">2</span></span>|<span data-ttu-id="d6c5a-121">所有支持外部 DMA 的 PCIe 设备将在任何时候枚举。</span><span class="sxs-lookup"><span data-stu-id="d6c5a-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



