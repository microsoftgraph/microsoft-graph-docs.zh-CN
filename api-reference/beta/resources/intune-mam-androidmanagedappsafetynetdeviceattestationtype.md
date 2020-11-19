---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6d5a94767f9a0e149a3b804bc805d94a66e92e70
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298013"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="993bd-103">androidManagedAppSafetyNetDeviceAttestationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="993bd-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="993bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="993bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="993bd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="993bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="993bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="993bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="993bd-107">管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。</span><span class="sxs-lookup"><span data-stu-id="993bd-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="993bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="993bd-108">Members</span></span>
|<span data-ttu-id="993bd-109">成员</span><span class="sxs-lookup"><span data-stu-id="993bd-109">Member</span></span>|<span data-ttu-id="993bd-110">值</span><span class="sxs-lookup"><span data-stu-id="993bd-110">Value</span></span>|<span data-ttu-id="993bd-111">Description</span><span class="sxs-lookup"><span data-stu-id="993bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="993bd-112">无</span><span class="sxs-lookup"><span data-stu-id="993bd-112">none</span></span>|<span data-ttu-id="993bd-113">0</span><span class="sxs-lookup"><span data-stu-id="993bd-113">0</span></span>|<span data-ttu-id="993bd-114">无要求集</span><span class="sxs-lookup"><span data-stu-id="993bd-114">no requirement set</span></span>|
|<span data-ttu-id="993bd-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="993bd-115">basicIntegrity</span></span>|<span data-ttu-id="993bd-116">1</span><span class="sxs-lookup"><span data-stu-id="993bd-116">1</span></span>|<span data-ttu-id="993bd-117">要求 Android 设备通过 SafetyNet 基本完整性验证</span><span class="sxs-lookup"><span data-stu-id="993bd-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="993bd-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="993bd-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="993bd-119">双面</span><span class="sxs-lookup"><span data-stu-id="993bd-119">2</span></span>|<span data-ttu-id="993bd-120">要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证</span><span class="sxs-lookup"><span data-stu-id="993bd-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|




