---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a75a8fda81c4169051c8b12fae9c1f7ece07795
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631464"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="d0b2a-103">androidManagedAppSafetyNetDeviceAttestationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d0b2a-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="d0b2a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0b2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0b2a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0b2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0b2a-106">管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。</span><span class="sxs-lookup"><span data-stu-id="d0b2a-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="d0b2a-107">成员</span><span class="sxs-lookup"><span data-stu-id="d0b2a-107">Members</span></span>
|<span data-ttu-id="d0b2a-108">成员</span><span class="sxs-lookup"><span data-stu-id="d0b2a-108">Member</span></span>|<span data-ttu-id="d0b2a-109">值</span><span class="sxs-lookup"><span data-stu-id="d0b2a-109">Value</span></span>|<span data-ttu-id="d0b2a-110">说明</span><span class="sxs-lookup"><span data-stu-id="d0b2a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0b2a-111">无</span><span class="sxs-lookup"><span data-stu-id="d0b2a-111">none</span></span>|<span data-ttu-id="d0b2a-112">0</span><span class="sxs-lookup"><span data-stu-id="d0b2a-112">0</span></span>|<span data-ttu-id="d0b2a-113">无要求集</span><span class="sxs-lookup"><span data-stu-id="d0b2a-113">no requirement set</span></span>|
|<span data-ttu-id="d0b2a-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="d0b2a-114">basicIntegrity</span></span>|<span data-ttu-id="d0b2a-115">1</span><span class="sxs-lookup"><span data-stu-id="d0b2a-115">1</span></span>|<span data-ttu-id="d0b2a-116">要求 Android 设备通过 SafetyNet 基本完整性验证</span><span class="sxs-lookup"><span data-stu-id="d0b2a-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="d0b2a-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="d0b2a-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="d0b2a-118">双面</span><span class="sxs-lookup"><span data-stu-id="d0b2a-118">2</span></span>|<span data-ttu-id="d0b2a-119">要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证</span><span class="sxs-lookup"><span data-stu-id="d0b2a-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|




