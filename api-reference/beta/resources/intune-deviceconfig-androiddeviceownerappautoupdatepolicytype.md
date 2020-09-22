---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者设备的应用自动更新策略状态的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5460053da38a09fdc4df4de0b4030b9081c19d0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076104"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="4bc6e-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4bc6e-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="4bc6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bc6e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bc6e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc6e-107">Android 设备所有者设备的应用自动更新策略状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="4bc6e-108">成员</span><span class="sxs-lookup"><span data-stu-id="4bc6e-108">Members</span></span>
|<span data-ttu-id="4bc6e-109">成员</span><span class="sxs-lookup"><span data-stu-id="4bc6e-109">Member</span></span>|<span data-ttu-id="4bc6e-110">值</span><span class="sxs-lookup"><span data-stu-id="4bc6e-110">Value</span></span>|<span data-ttu-id="4bc6e-111">说明</span><span class="sxs-lookup"><span data-stu-id="4bc6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc6e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4bc6e-112">notConfigured</span></span>|<span data-ttu-id="4bc6e-113">0</span><span class="sxs-lookup"><span data-stu-id="4bc6e-113">0</span></span>|<span data-ttu-id="4bc6e-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="4bc6e-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="4bc6e-115">userChoice</span></span>|<span data-ttu-id="4bc6e-116">1 </span><span class="sxs-lookup"><span data-stu-id="4bc6e-116">1</span></span>|<span data-ttu-id="4bc6e-117">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="4bc6e-118">永不</span><span class="sxs-lookup"><span data-stu-id="4bc6e-118">never</span></span>|<span data-ttu-id="4bc6e-119">2 </span><span class="sxs-lookup"><span data-stu-id="4bc6e-119">2</span></span>|<span data-ttu-id="4bc6e-120">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="4bc6e-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="4bc6e-121">wiFiOnly</span></span>|<span data-ttu-id="4bc6e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="4bc6e-122">3</span></span>|<span data-ttu-id="4bc6e-123">仅通过 Wi-fi 自动更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="4bc6e-124">都</span><span class="sxs-lookup"><span data-stu-id="4bc6e-124">always</span></span>|<span data-ttu-id="4bc6e-125">4 </span><span class="sxs-lookup"><span data-stu-id="4bc6e-125">4</span></span>|<span data-ttu-id="4bc6e-126">应用将在任何时候自动更新。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="4bc6e-127">可能会收取数据费用。</span><span class="sxs-lookup"><span data-stu-id="4bc6e-127">Data charges may apply.</span></span>|






