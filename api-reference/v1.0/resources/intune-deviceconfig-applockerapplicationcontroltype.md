---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575126"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="09c92-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="09c92-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="09c92-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09c92-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09c92-105">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="09c92-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="09c92-106">成员</span><span class="sxs-lookup"><span data-stu-id="09c92-106">Members</span></span>
|<span data-ttu-id="09c92-107">成员</span><span class="sxs-lookup"><span data-stu-id="09c92-107">Member</span></span>|<span data-ttu-id="09c92-108">值</span><span class="sxs-lookup"><span data-stu-id="09c92-108">Value</span></span>|<span data-ttu-id="09c92-109">说明</span><span class="sxs-lookup"><span data-stu-id="09c92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09c92-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="09c92-110">notConfigured</span></span>|<span data-ttu-id="09c92-111">0</span><span class="sxs-lookup"><span data-stu-id="09c92-111">0</span></span>|<span data-ttu-id="09c92-112">设备默认值, 未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="09c92-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="09c92-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="09c92-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="09c92-114">1</span><span class="sxs-lookup"><span data-stu-id="09c92-114">1</span></span>|<span data-ttu-id="09c92-115">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="09c92-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="09c92-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="09c92-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="09c92-117">2 </span><span class="sxs-lookup"><span data-stu-id="09c92-117">2</span></span>|<span data-ttu-id="09c92-118">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="09c92-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="09c92-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="09c92-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="09c92-120">3 </span><span class="sxs-lookup"><span data-stu-id="09c92-120">3</span></span>|<span data-ttu-id="09c92-121">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="09c92-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="09c92-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="09c92-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="09c92-123">4 </span><span class="sxs-lookup"><span data-stu-id="09c92-123">4</span></span>|<span data-ttu-id="09c92-124">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="09c92-124">Audit Windows components, store apps and smart locker.</span></span>|



