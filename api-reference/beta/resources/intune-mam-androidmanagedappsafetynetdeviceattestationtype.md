---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 285389d07f4ea6f667a0e12260fe5a5296808923
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524362"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="dbb11-103">androidManagedAppSafetyNetDeviceAttestationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dbb11-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="dbb11-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dbb11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbb11-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dbb11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbb11-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbb11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbb11-107">管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。</span><span class="sxs-lookup"><span data-stu-id="dbb11-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="dbb11-108">成员</span><span class="sxs-lookup"><span data-stu-id="dbb11-108">Members</span></span>
|<span data-ttu-id="dbb11-109">成员</span><span class="sxs-lookup"><span data-stu-id="dbb11-109">Member</span></span>|<span data-ttu-id="dbb11-110">值</span><span class="sxs-lookup"><span data-stu-id="dbb11-110">Value</span></span>|<span data-ttu-id="dbb11-111">说明</span><span class="sxs-lookup"><span data-stu-id="dbb11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb11-112">无</span><span class="sxs-lookup"><span data-stu-id="dbb11-112">none</span></span>|<span data-ttu-id="dbb11-113">0</span><span class="sxs-lookup"><span data-stu-id="dbb11-113">0</span></span>|<span data-ttu-id="dbb11-114">无要求集</span><span class="sxs-lookup"><span data-stu-id="dbb11-114">no requirement set</span></span>|
|<span data-ttu-id="dbb11-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="dbb11-115">basicIntegrity</span></span>|<span data-ttu-id="dbb11-116">1 </span><span class="sxs-lookup"><span data-stu-id="dbb11-116">1</span></span>|<span data-ttu-id="dbb11-117">要求 Android 设备通过 SafetyNet 基本完整性验证</span><span class="sxs-lookup"><span data-stu-id="dbb11-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="dbb11-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="dbb11-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="dbb11-119">2 </span><span class="sxs-lookup"><span data-stu-id="dbb11-119">2</span></span>|<span data-ttu-id="dbb11-120">要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证</span><span class="sxs-lookup"><span data-stu-id="dbb11-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



