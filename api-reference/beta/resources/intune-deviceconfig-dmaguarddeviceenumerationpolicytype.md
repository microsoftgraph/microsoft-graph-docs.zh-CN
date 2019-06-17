---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4e534fca412c6d48ab9ea006f308a114c73def2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989915"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="f3c93-103">dmaGuardDeviceEnumerationPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f3c93-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="f3c93-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3c93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3c93-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3c93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3c93-106">DmaGuardDeviceEnumerationPolicy 的可能值。</span><span class="sxs-lookup"><span data-stu-id="f3c93-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="f3c93-107">成员</span><span class="sxs-lookup"><span data-stu-id="f3c93-107">Members</span></span>
|<span data-ttu-id="f3c93-108">成员</span><span class="sxs-lookup"><span data-stu-id="f3c93-108">Member</span></span>|<span data-ttu-id="f3c93-109">值</span><span class="sxs-lookup"><span data-stu-id="f3c93-109">Value</span></span>|<span data-ttu-id="f3c93-110">说明</span><span class="sxs-lookup"><span data-stu-id="f3c93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c93-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f3c93-111">deviceDefault</span></span>|<span data-ttu-id="f3c93-112">0</span><span class="sxs-lookup"><span data-stu-id="f3c93-112">0</span></span>|<span data-ttu-id="f3c93-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="f3c93-113">Default value.</span></span> <span data-ttu-id="f3c93-114">具有 DMA 重新映射的设备将仅在用户解锁屏幕后枚举不兼容驱动程序。</span><span class="sxs-lookup"><span data-stu-id="f3c93-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="f3c93-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="f3c93-115">blockAll</span></span>|<span data-ttu-id="f3c93-116">1</span><span class="sxs-lookup"><span data-stu-id="f3c93-116">1</span></span>|<span data-ttu-id="f3c93-117">具有 DMA 重新映射的设备不支持的驱动程序在任何时候都不能随时启动和执行 DMA。</span><span class="sxs-lookup"><span data-stu-id="f3c93-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="f3c93-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="f3c93-118">allowAll</span></span>|<span data-ttu-id="f3c93-119">双面</span><span class="sxs-lookup"><span data-stu-id="f3c93-119">2</span></span>|<span data-ttu-id="f3c93-120">所有支持外部 DMA 的 PCIe 设备将在任何时候枚举。</span><span class="sxs-lookup"><span data-stu-id="f3c93-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





