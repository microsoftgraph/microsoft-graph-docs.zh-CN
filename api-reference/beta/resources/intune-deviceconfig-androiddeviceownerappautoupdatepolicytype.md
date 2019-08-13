---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者设备的应用自动更新策略状态的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3491d175f4157bae2229277e35ea937741d06324
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334862"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="12ca4-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12ca4-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="12ca4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12ca4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12ca4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12ca4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12ca4-106">Android 设备所有者设备的应用自动更新策略状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="12ca4-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="12ca4-107">成员</span><span class="sxs-lookup"><span data-stu-id="12ca4-107">Members</span></span>
|<span data-ttu-id="12ca4-108">成员</span><span class="sxs-lookup"><span data-stu-id="12ca4-108">Member</span></span>|<span data-ttu-id="12ca4-109">值</span><span class="sxs-lookup"><span data-stu-id="12ca4-109">Value</span></span>|<span data-ttu-id="12ca4-110">说明</span><span class="sxs-lookup"><span data-stu-id="12ca4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ca4-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="12ca4-111">notConfigured</span></span>|<span data-ttu-id="12ca4-112">0</span><span class="sxs-lookup"><span data-stu-id="12ca4-112">0</span></span>|<span data-ttu-id="12ca4-113">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="12ca4-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="12ca4-114">userChoice</span><span class="sxs-lookup"><span data-stu-id="12ca4-114">userChoice</span></span>|<span data-ttu-id="12ca4-115">1</span><span class="sxs-lookup"><span data-stu-id="12ca4-115">1</span></span>|<span data-ttu-id="12ca4-116">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="12ca4-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="12ca4-117">永不</span><span class="sxs-lookup"><span data-stu-id="12ca4-117">never</span></span>|<span data-ttu-id="12ca4-118">双面</span><span class="sxs-lookup"><span data-stu-id="12ca4-118">2</span></span>|<span data-ttu-id="12ca4-119">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="12ca4-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="12ca4-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="12ca4-120">wiFiOnly</span></span>|<span data-ttu-id="12ca4-121">第三章</span><span class="sxs-lookup"><span data-stu-id="12ca4-121">3</span></span>|<span data-ttu-id="12ca4-122">仅通过 Wi-fi 自动更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="12ca4-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="12ca4-123">都</span><span class="sxs-lookup"><span data-stu-id="12ca4-123">always</span></span>|<span data-ttu-id="12ca4-124">4</span><span class="sxs-lookup"><span data-stu-id="12ca4-124">4</span></span>|<span data-ttu-id="12ca4-125">应用将在任何时候自动更新。</span><span class="sxs-lookup"><span data-stu-id="12ca4-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="12ca4-126">可能会收取数据费用。</span><span class="sxs-lookup"><span data-stu-id="12ca4-126">Data charges may apply.</span></span>|



