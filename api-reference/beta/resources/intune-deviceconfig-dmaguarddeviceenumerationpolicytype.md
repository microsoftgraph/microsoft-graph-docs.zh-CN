---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429482"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="21f4a-103">dmaGuardDeviceEnumerationPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21f4a-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="21f4a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="21f4a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21f4a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21f4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21f4a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21f4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21f4a-107">DmaGuardDeviceEnumerationPolicy 的可能值。</span><span class="sxs-lookup"><span data-stu-id="21f4a-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="21f4a-108">成员</span><span class="sxs-lookup"><span data-stu-id="21f4a-108">Members</span></span>
|<span data-ttu-id="21f4a-109">成员</span><span class="sxs-lookup"><span data-stu-id="21f4a-109">Member</span></span>|<span data-ttu-id="21f4a-110">值</span><span class="sxs-lookup"><span data-stu-id="21f4a-110">Value</span></span>|<span data-ttu-id="21f4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="21f4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21f4a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="21f4a-112">deviceDefault</span></span>|<span data-ttu-id="21f4a-113">0</span><span class="sxs-lookup"><span data-stu-id="21f4a-113">0</span></span>|<span data-ttu-id="21f4a-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="21f4a-114">Default value.</span></span> <span data-ttu-id="21f4a-115">用户解除锁定的屏幕后，将仅枚举设备 DMA 重新映射不兼容的驱动程序。</span><span class="sxs-lookup"><span data-stu-id="21f4a-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="21f4a-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="21f4a-116">blockAll</span></span>|<span data-ttu-id="21f4a-117">1</span><span class="sxs-lookup"><span data-stu-id="21f4a-117">1</span></span>|<span data-ttu-id="21f4a-118">从不允许设备 DMA 重新映射不兼容的驱动程序启动并随时执行 DMA。</span><span class="sxs-lookup"><span data-stu-id="21f4a-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="21f4a-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="21f4a-119">allowAll</span></span>|<span data-ttu-id="21f4a-120">2</span><span class="sxs-lookup"><span data-stu-id="21f4a-120">2</span></span>|<span data-ttu-id="21f4a-121">在任何时候都将被枚举所有外部的 DMA 能够 PCIe 设备。</span><span class="sxs-lookup"><span data-stu-id="21f4a-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




