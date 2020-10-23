---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4be968bfb2191b71fd810ee83ce36d4e795ea17b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730309"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="00a7b-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="00a7b-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="00a7b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00a7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00a7b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00a7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00a7b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00a7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00a7b-107">指示设备上的移动应用的状态。</span><span class="sxs-lookup"><span data-stu-id="00a7b-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="00a7b-108">成员</span><span class="sxs-lookup"><span data-stu-id="00a7b-108">Members</span></span>
|<span data-ttu-id="00a7b-109">成员</span><span class="sxs-lookup"><span data-stu-id="00a7b-109">Member</span></span>|<span data-ttu-id="00a7b-110">值</span><span class="sxs-lookup"><span data-stu-id="00a7b-110">Value</span></span>|<span data-ttu-id="00a7b-111">说明</span><span class="sxs-lookup"><span data-stu-id="00a7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a7b-112">可用</span><span class="sxs-lookup"><span data-stu-id="00a7b-112">available</span></span>|<span data-ttu-id="00a7b-113">0</span><span class="sxs-lookup"><span data-stu-id="00a7b-113">0</span></span>|<span data-ttu-id="00a7b-114">可用</span><span class="sxs-lookup"><span data-stu-id="00a7b-114">Available</span></span>|
|<span data-ttu-id="00a7b-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="00a7b-115">notAvailable</span></span>|<span data-ttu-id="00a7b-116">1</span><span class="sxs-lookup"><span data-stu-id="00a7b-116">1</span></span>|<span data-ttu-id="00a7b-117">不可用</span><span class="sxs-lookup"><span data-stu-id="00a7b-117">Not Available</span></span>|
|<span data-ttu-id="00a7b-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="00a7b-118">requiredInstall</span></span>|<span data-ttu-id="00a7b-119">双面</span><span class="sxs-lookup"><span data-stu-id="00a7b-119">2</span></span>|<span data-ttu-id="00a7b-120">必需的安装</span><span class="sxs-lookup"><span data-stu-id="00a7b-120">Required Install</span></span>|
|<span data-ttu-id="00a7b-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="00a7b-121">requiredUninstall</span></span>|<span data-ttu-id="00a7b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="00a7b-122">3</span></span>|<span data-ttu-id="00a7b-123">必需的卸载</span><span class="sxs-lookup"><span data-stu-id="00a7b-123">Required Uninstall</span></span>|
|<span data-ttu-id="00a7b-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="00a7b-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="00a7b-125">4 </span><span class="sxs-lookup"><span data-stu-id="00a7b-125">4</span></span>|<span data-ttu-id="00a7b-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="00a7b-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="00a7b-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="00a7b-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="00a7b-128">5 </span><span class="sxs-lookup"><span data-stu-id="00a7b-128">5</span></span>|<span data-ttu-id="00a7b-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="00a7b-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="00a7b-130">排除</span><span class="sxs-lookup"><span data-stu-id="00a7b-130">exclude</span></span>|<span data-ttu-id="00a7b-131">6 </span><span class="sxs-lookup"><span data-stu-id="00a7b-131">6</span></span>|<span data-ttu-id="00a7b-132">排除</span><span class="sxs-lookup"><span data-stu-id="00a7b-132">Exclude</span></span>|





