---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者设备的应用自动更新策略状态的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd003c8213faf45453f1b6165931181250c861ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487198"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="b9466-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b9466-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="b9466-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b9466-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9466-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9466-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9466-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9466-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9466-107">Android 设备所有者设备的应用自动更新策略状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="b9466-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="b9466-108">成员</span><span class="sxs-lookup"><span data-stu-id="b9466-108">Members</span></span>
|<span data-ttu-id="b9466-109">成员</span><span class="sxs-lookup"><span data-stu-id="b9466-109">Member</span></span>|<span data-ttu-id="b9466-110">值</span><span class="sxs-lookup"><span data-stu-id="b9466-110">Value</span></span>|<span data-ttu-id="b9466-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9466-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9466-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b9466-112">notConfigured</span></span>|<span data-ttu-id="b9466-113">0</span><span class="sxs-lookup"><span data-stu-id="b9466-113">0</span></span>|<span data-ttu-id="b9466-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="b9466-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="b9466-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="b9466-115">userChoice</span></span>|<span data-ttu-id="b9466-116">1 </span><span class="sxs-lookup"><span data-stu-id="b9466-116">1</span></span>|<span data-ttu-id="b9466-117">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="b9466-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="b9466-118">永不</span><span class="sxs-lookup"><span data-stu-id="b9466-118">never</span></span>|<span data-ttu-id="b9466-119">2 </span><span class="sxs-lookup"><span data-stu-id="b9466-119">2</span></span>|<span data-ttu-id="b9466-120">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="b9466-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="b9466-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="b9466-121">wiFiOnly</span></span>|<span data-ttu-id="b9466-122">3 </span><span class="sxs-lookup"><span data-stu-id="b9466-122">3</span></span>|<span data-ttu-id="b9466-123">仅通过 Wi-fi 自动更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="b9466-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="b9466-124">都</span><span class="sxs-lookup"><span data-stu-id="b9466-124">always</span></span>|<span data-ttu-id="b9466-125">4 </span><span class="sxs-lookup"><span data-stu-id="b9466-125">4</span></span>|<span data-ttu-id="b9466-126">应用将在任何时候自动更新。</span><span class="sxs-lookup"><span data-stu-id="b9466-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="b9466-127">可能会收取数据费用。</span><span class="sxs-lookup"><span data-stu-id="b9466-127">Data charges may apply.</span></span>|



