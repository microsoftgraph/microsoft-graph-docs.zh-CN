---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e3289a40916d4942980274e2375aefdf6081934c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791966"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="39125-103">dmaGuardDeviceEnumerationPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="39125-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="39125-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="39125-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39125-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39125-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39125-106">DmaGuardDeviceEnumerationPolicy 的可能值。</span><span class="sxs-lookup"><span data-stu-id="39125-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="39125-107">成员</span><span class="sxs-lookup"><span data-stu-id="39125-107">Members</span></span>
|<span data-ttu-id="39125-108">成员</span><span class="sxs-lookup"><span data-stu-id="39125-108">Member</span></span>|<span data-ttu-id="39125-109">值</span><span class="sxs-lookup"><span data-stu-id="39125-109">Value</span></span>|<span data-ttu-id="39125-110">说明</span><span class="sxs-lookup"><span data-stu-id="39125-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39125-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="39125-111">deviceDefault</span></span>|<span data-ttu-id="39125-112">0</span><span class="sxs-lookup"><span data-stu-id="39125-112">0</span></span>|<span data-ttu-id="39125-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="39125-113">Default value.</span></span> <span data-ttu-id="39125-114">具有 DMA 重新映射的设备将仅在用户解锁屏幕后枚举不兼容驱动程序。</span><span class="sxs-lookup"><span data-stu-id="39125-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="39125-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="39125-115">blockAll</span></span>|<span data-ttu-id="39125-116">1</span><span class="sxs-lookup"><span data-stu-id="39125-116">1</span></span>|<span data-ttu-id="39125-117">具有 DMA 重新映射的设备不支持的驱动程序在任何时候都不能随时启动和执行 DMA。</span><span class="sxs-lookup"><span data-stu-id="39125-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="39125-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="39125-118">allowAll</span></span>|<span data-ttu-id="39125-119">双面</span><span class="sxs-lookup"><span data-stu-id="39125-119">2</span></span>|<span data-ttu-id="39125-120">所有支持外部 DMA 的 PCIe 设备将在任何时候枚举。</span><span class="sxs-lookup"><span data-stu-id="39125-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



