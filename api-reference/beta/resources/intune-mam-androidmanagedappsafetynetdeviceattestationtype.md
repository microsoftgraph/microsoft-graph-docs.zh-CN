---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f18a4eb3dd7d31c51dc21a02999aa4ea99d2f0fd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723875"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="a9b61-103">androidManagedAppSafetyNetDeviceAttestationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a9b61-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="a9b61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9b61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9b61-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9b61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9b61-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9b61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b61-107">管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。</span><span class="sxs-lookup"><span data-stu-id="a9b61-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="a9b61-108">成员</span><span class="sxs-lookup"><span data-stu-id="a9b61-108">Members</span></span>
|<span data-ttu-id="a9b61-109">成员</span><span class="sxs-lookup"><span data-stu-id="a9b61-109">Member</span></span>|<span data-ttu-id="a9b61-110">值</span><span class="sxs-lookup"><span data-stu-id="a9b61-110">Value</span></span>|<span data-ttu-id="a9b61-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9b61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b61-112">无</span><span class="sxs-lookup"><span data-stu-id="a9b61-112">none</span></span>|<span data-ttu-id="a9b61-113">0</span><span class="sxs-lookup"><span data-stu-id="a9b61-113">0</span></span>|<span data-ttu-id="a9b61-114">无要求集</span><span class="sxs-lookup"><span data-stu-id="a9b61-114">no requirement set</span></span>|
|<span data-ttu-id="a9b61-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="a9b61-115">basicIntegrity</span></span>|<span data-ttu-id="a9b61-116">1</span><span class="sxs-lookup"><span data-stu-id="a9b61-116">1</span></span>|<span data-ttu-id="a9b61-117">要求 Android 设备通过 SafetyNet 基本完整性验证</span><span class="sxs-lookup"><span data-stu-id="a9b61-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="a9b61-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="a9b61-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="a9b61-119">双面</span><span class="sxs-lookup"><span data-stu-id="a9b61-119">2</span></span>|<span data-ttu-id="a9b61-120">要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证</span><span class="sxs-lookup"><span data-stu-id="a9b61-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





