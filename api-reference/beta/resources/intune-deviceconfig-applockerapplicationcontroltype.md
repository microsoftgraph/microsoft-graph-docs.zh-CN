---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 076ce5f69fd49fa95bab6dbf5ee8dc00eea39488
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075929"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="cba93-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cba93-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="cba93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cba93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cba93-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cba93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cba93-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cba93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cba93-107">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="cba93-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="cba93-108">成员</span><span class="sxs-lookup"><span data-stu-id="cba93-108">Members</span></span>
|<span data-ttu-id="cba93-109">成员</span><span class="sxs-lookup"><span data-stu-id="cba93-109">Member</span></span>|<span data-ttu-id="cba93-110">值</span><span class="sxs-lookup"><span data-stu-id="cba93-110">Value</span></span>|<span data-ttu-id="cba93-111">说明</span><span class="sxs-lookup"><span data-stu-id="cba93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba93-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cba93-112">notConfigured</span></span>|<span data-ttu-id="cba93-113">0</span><span class="sxs-lookup"><span data-stu-id="cba93-113">0</span></span>|<span data-ttu-id="cba93-114">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="cba93-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="cba93-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="cba93-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="cba93-116">1 </span><span class="sxs-lookup"><span data-stu-id="cba93-116">1</span></span>|<span data-ttu-id="cba93-117">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="cba93-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="cba93-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="cba93-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="cba93-119">2 </span><span class="sxs-lookup"><span data-stu-id="cba93-119">2</span></span>|<span data-ttu-id="cba93-120">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="cba93-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="cba93-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="cba93-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="cba93-122">第三章</span><span class="sxs-lookup"><span data-stu-id="cba93-122">3</span></span>|<span data-ttu-id="cba93-123">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="cba93-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="cba93-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="cba93-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="cba93-125">4 </span><span class="sxs-lookup"><span data-stu-id="cba93-125">4</span></span>|<span data-ttu-id="cba93-126">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="cba93-126">Audit Windows components, store apps and smart locker.</span></span>|






