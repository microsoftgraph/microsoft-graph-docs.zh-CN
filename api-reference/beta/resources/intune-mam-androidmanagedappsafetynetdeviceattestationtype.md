---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 645027397a852c98ee973ee53382e4e552724ab0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030561"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="ffd15-103">androidManagedAppSafetyNetDeviceAttestationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ffd15-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="ffd15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffd15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffd15-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffd15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffd15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffd15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffd15-107">管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。</span><span class="sxs-lookup"><span data-stu-id="ffd15-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="ffd15-108">成员</span><span class="sxs-lookup"><span data-stu-id="ffd15-108">Members</span></span>
|<span data-ttu-id="ffd15-109">成员</span><span class="sxs-lookup"><span data-stu-id="ffd15-109">Member</span></span>|<span data-ttu-id="ffd15-110">值</span><span class="sxs-lookup"><span data-stu-id="ffd15-110">Value</span></span>|<span data-ttu-id="ffd15-111">说明</span><span class="sxs-lookup"><span data-stu-id="ffd15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd15-112">无</span><span class="sxs-lookup"><span data-stu-id="ffd15-112">none</span></span>|<span data-ttu-id="ffd15-113">0</span><span class="sxs-lookup"><span data-stu-id="ffd15-113">0</span></span>|<span data-ttu-id="ffd15-114">无要求集</span><span class="sxs-lookup"><span data-stu-id="ffd15-114">no requirement set</span></span>|
|<span data-ttu-id="ffd15-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="ffd15-115">basicIntegrity</span></span>|<span data-ttu-id="ffd15-116">1 </span><span class="sxs-lookup"><span data-stu-id="ffd15-116">1</span></span>|<span data-ttu-id="ffd15-117">要求 Android 设备通过 SafetyNet 基本完整性验证</span><span class="sxs-lookup"><span data-stu-id="ffd15-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="ffd15-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="ffd15-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="ffd15-119">2 </span><span class="sxs-lookup"><span data-stu-id="ffd15-119">2</span></span>|<span data-ttu-id="ffd15-120">要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证</span><span class="sxs-lookup"><span data-stu-id="ffd15-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|






