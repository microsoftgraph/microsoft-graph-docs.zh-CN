---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者设备的应用自动更新策略状态的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bdc8c5f9064ab68017d9857f384fb17388d0cce7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971548"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="eb982-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="eb982-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="eb982-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb982-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb982-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb982-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb982-106">Android 设备所有者设备的应用自动更新策略状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="eb982-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="eb982-107">成员</span><span class="sxs-lookup"><span data-stu-id="eb982-107">Members</span></span>
|<span data-ttu-id="eb982-108">成员</span><span class="sxs-lookup"><span data-stu-id="eb982-108">Member</span></span>|<span data-ttu-id="eb982-109">值</span><span class="sxs-lookup"><span data-stu-id="eb982-109">Value</span></span>|<span data-ttu-id="eb982-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb982-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb982-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="eb982-111">notConfigured</span></span>|<span data-ttu-id="eb982-112">0</span><span class="sxs-lookup"><span data-stu-id="eb982-112">0</span></span>|<span data-ttu-id="eb982-113">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="eb982-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="eb982-114">userChoice</span><span class="sxs-lookup"><span data-stu-id="eb982-114">userChoice</span></span>|<span data-ttu-id="eb982-115">1</span><span class="sxs-lookup"><span data-stu-id="eb982-115">1</span></span>|<span data-ttu-id="eb982-116">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="eb982-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="eb982-117">永不</span><span class="sxs-lookup"><span data-stu-id="eb982-117">never</span></span>|<span data-ttu-id="eb982-118">双面</span><span class="sxs-lookup"><span data-stu-id="eb982-118">2</span></span>|<span data-ttu-id="eb982-119">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="eb982-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="eb982-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="eb982-120">wiFiOnly</span></span>|<span data-ttu-id="eb982-121">第三章</span><span class="sxs-lookup"><span data-stu-id="eb982-121">3</span></span>|<span data-ttu-id="eb982-122">仅通过 Wi-fi 自动更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb982-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="eb982-123">都</span><span class="sxs-lookup"><span data-stu-id="eb982-123">always</span></span>|<span data-ttu-id="eb982-124">4</span><span class="sxs-lookup"><span data-stu-id="eb982-124">4</span></span>|<span data-ttu-id="eb982-125">应用将在任何时候自动更新。</span><span class="sxs-lookup"><span data-stu-id="eb982-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="eb982-126">可能会收取数据费用。</span><span class="sxs-lookup"><span data-stu-id="eb982-126">Data charges may apply.</span></span>|





