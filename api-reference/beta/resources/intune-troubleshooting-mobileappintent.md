---
title: mobileAppIntent 枚举类型
description: 指示在设备上的移动应用程序的状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a807e89ec949c2c48f04af46b26f43b393cc4b0a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419259"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="a3217-103">mobileAppIntent 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3217-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="a3217-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a3217-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3217-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3217-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3217-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3217-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3217-107">指示在设备上的移动应用程序的状态。</span><span class="sxs-lookup"><span data-stu-id="a3217-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="a3217-108">成员</span><span class="sxs-lookup"><span data-stu-id="a3217-108">Members</span></span>
|<span data-ttu-id="a3217-109">成员</span><span class="sxs-lookup"><span data-stu-id="a3217-109">Member</span></span>|<span data-ttu-id="a3217-110">值</span><span class="sxs-lookup"><span data-stu-id="a3217-110">Value</span></span>|<span data-ttu-id="a3217-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3217-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3217-112">可用</span><span class="sxs-lookup"><span data-stu-id="a3217-112">available</span></span>|<span data-ttu-id="a3217-113">0</span><span class="sxs-lookup"><span data-stu-id="a3217-113">0</span></span>|<span data-ttu-id="a3217-114">可用</span><span class="sxs-lookup"><span data-stu-id="a3217-114">Available</span></span>|
|<span data-ttu-id="a3217-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="a3217-115">notAvailable</span></span>|<span data-ttu-id="a3217-116">1</span><span class="sxs-lookup"><span data-stu-id="a3217-116">1</span></span>|<span data-ttu-id="a3217-117">不可用</span><span class="sxs-lookup"><span data-stu-id="a3217-117">Not Available</span></span>|
|<span data-ttu-id="a3217-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="a3217-118">requiredInstall</span></span>|<span data-ttu-id="a3217-119">2</span><span class="sxs-lookup"><span data-stu-id="a3217-119">2</span></span>|<span data-ttu-id="a3217-120">所需的安装</span><span class="sxs-lookup"><span data-stu-id="a3217-120">Required Install</span></span>|
|<span data-ttu-id="a3217-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="a3217-121">requiredUninstall</span></span>|<span data-ttu-id="a3217-122">3</span><span class="sxs-lookup"><span data-stu-id="a3217-122">3</span></span>|<span data-ttu-id="a3217-123">需要的卸载</span><span class="sxs-lookup"><span data-stu-id="a3217-123">Required Uninstall</span></span>|
|<span data-ttu-id="a3217-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="a3217-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="a3217-125">4</span><span class="sxs-lookup"><span data-stu-id="a3217-125">4</span></span>|<span data-ttu-id="a3217-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="a3217-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="a3217-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="a3217-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="a3217-128">5</span><span class="sxs-lookup"><span data-stu-id="a3217-128">5</span></span>|<span data-ttu-id="a3217-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="a3217-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="a3217-130">排除</span><span class="sxs-lookup"><span data-stu-id="a3217-130">exclude</span></span>|<span data-ttu-id="a3217-131">6</span><span class="sxs-lookup"><span data-stu-id="a3217-131">6</span></span>|<span data-ttu-id="a3217-132">排除</span><span class="sxs-lookup"><span data-stu-id="a3217-132">Exclude</span></span>|




