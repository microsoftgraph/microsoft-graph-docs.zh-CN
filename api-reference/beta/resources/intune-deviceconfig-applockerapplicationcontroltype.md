---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4fab692743e0e76b37e81ff88e7a4d464c96e17
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799494"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="ab957-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab957-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="ab957-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab957-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab957-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab957-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab957-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="ab957-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="ab957-107">成员</span><span class="sxs-lookup"><span data-stu-id="ab957-107">Members</span></span>
|<span data-ttu-id="ab957-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab957-108">Member</span></span>|<span data-ttu-id="ab957-109">值</span><span class="sxs-lookup"><span data-stu-id="ab957-109">Value</span></span>|<span data-ttu-id="ab957-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab957-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab957-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ab957-111">notConfigured</span></span>|<span data-ttu-id="ab957-112">0</span><span class="sxs-lookup"><span data-stu-id="ab957-112">0</span></span>|<span data-ttu-id="ab957-113">设备默认值, 未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="ab957-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="ab957-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ab957-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="ab957-115">1</span><span class="sxs-lookup"><span data-stu-id="ab957-115">1</span></span>|<span data-ttu-id="ab957-116">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="ab957-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="ab957-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ab957-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="ab957-118">双面</span><span class="sxs-lookup"><span data-stu-id="ab957-118">2</span></span>|<span data-ttu-id="ab957-119">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab957-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="ab957-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ab957-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ab957-121">第三章</span><span class="sxs-lookup"><span data-stu-id="ab957-121">3</span></span>|<span data-ttu-id="ab957-122">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="ab957-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="ab957-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ab957-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ab957-124">4</span><span class="sxs-lookup"><span data-stu-id="ab957-124">4</span></span>|<span data-ttu-id="ab957-125">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="ab957-125">Audit Windows components, store apps and smart locker.</span></span>|





