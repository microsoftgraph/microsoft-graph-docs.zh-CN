---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 93d65431cfcdfc952231237f2646eee79e331ef3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782697"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="b24c8-103">androidManagedAppSafetyNetDeviceAttestationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b24c8-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="b24c8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b24c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b24c8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b24c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b24c8-106">管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。</span><span class="sxs-lookup"><span data-stu-id="b24c8-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="b24c8-107">成员</span><span class="sxs-lookup"><span data-stu-id="b24c8-107">Members</span></span>
|<span data-ttu-id="b24c8-108">成员</span><span class="sxs-lookup"><span data-stu-id="b24c8-108">Member</span></span>|<span data-ttu-id="b24c8-109">值</span><span class="sxs-lookup"><span data-stu-id="b24c8-109">Value</span></span>|<span data-ttu-id="b24c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="b24c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b24c8-111">无</span><span class="sxs-lookup"><span data-stu-id="b24c8-111">none</span></span>|<span data-ttu-id="b24c8-112">0</span><span class="sxs-lookup"><span data-stu-id="b24c8-112">0</span></span>|<span data-ttu-id="b24c8-113">无要求集</span><span class="sxs-lookup"><span data-stu-id="b24c8-113">no requirement set</span></span>|
|<span data-ttu-id="b24c8-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b24c8-114">basicIntegrity</span></span>|<span data-ttu-id="b24c8-115">1</span><span class="sxs-lookup"><span data-stu-id="b24c8-115">1</span></span>|<span data-ttu-id="b24c8-116">要求 Android 设备通过 SafetyNet 基本完整性验证</span><span class="sxs-lookup"><span data-stu-id="b24c8-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="b24c8-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="b24c8-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="b24c8-118">双面</span><span class="sxs-lookup"><span data-stu-id="b24c8-118">2</span></span>|<span data-ttu-id="b24c8-119">要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证</span><span class="sxs-lookup"><span data-stu-id="b24c8-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



