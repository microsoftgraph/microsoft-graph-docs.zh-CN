---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e34472e8f534f78167d57309bd7315102bf8a3b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051093"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="30cf2-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="30cf2-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="30cf2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30cf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30cf2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30cf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30cf2-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="30cf2-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="30cf2-107">成员</span><span class="sxs-lookup"><span data-stu-id="30cf2-107">Members</span></span>
|<span data-ttu-id="30cf2-108">成员</span><span class="sxs-lookup"><span data-stu-id="30cf2-108">Member</span></span>|<span data-ttu-id="30cf2-109">值</span><span class="sxs-lookup"><span data-stu-id="30cf2-109">Value</span></span>|<span data-ttu-id="30cf2-110">说明</span><span class="sxs-lookup"><span data-stu-id="30cf2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30cf2-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="30cf2-111">notConfigured</span></span>|<span data-ttu-id="30cf2-112">0</span><span class="sxs-lookup"><span data-stu-id="30cf2-112">0</span></span>|<span data-ttu-id="30cf2-113">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="30cf2-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="30cf2-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="30cf2-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="30cf2-115">1 </span><span class="sxs-lookup"><span data-stu-id="30cf2-115">1</span></span>|<span data-ttu-id="30cf2-116">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="30cf2-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="30cf2-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="30cf2-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="30cf2-118">2 </span><span class="sxs-lookup"><span data-stu-id="30cf2-118">2</span></span>|<span data-ttu-id="30cf2-119">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="30cf2-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="30cf2-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="30cf2-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="30cf2-121">第三章</span><span class="sxs-lookup"><span data-stu-id="30cf2-121">3</span></span>|<span data-ttu-id="30cf2-122">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="30cf2-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="30cf2-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="30cf2-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="30cf2-124">4 </span><span class="sxs-lookup"><span data-stu-id="30cf2-124">4</span></span>|<span data-ttu-id="30cf2-125">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="30cf2-125">Audit Windows components, store apps and smart locker.</span></span>|









