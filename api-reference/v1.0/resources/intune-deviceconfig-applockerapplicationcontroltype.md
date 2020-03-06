---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ca428eb0ccf9121cc3a7b02e6abb333e0b4e5503
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530925"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="fd98a-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fd98a-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="fd98a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd98a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd98a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd98a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd98a-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="fd98a-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="fd98a-107">成员</span><span class="sxs-lookup"><span data-stu-id="fd98a-107">Members</span></span>
|<span data-ttu-id="fd98a-108">成员</span><span class="sxs-lookup"><span data-stu-id="fd98a-108">Member</span></span>|<span data-ttu-id="fd98a-109">值</span><span class="sxs-lookup"><span data-stu-id="fd98a-109">Value</span></span>|<span data-ttu-id="fd98a-110">说明</span><span class="sxs-lookup"><span data-stu-id="fd98a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd98a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fd98a-111">notConfigured</span></span>|<span data-ttu-id="fd98a-112">0</span><span class="sxs-lookup"><span data-stu-id="fd98a-112">0</span></span>|<span data-ttu-id="fd98a-113">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="fd98a-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="fd98a-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="fd98a-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="fd98a-115">1 </span><span class="sxs-lookup"><span data-stu-id="fd98a-115">1</span></span>|<span data-ttu-id="fd98a-116">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="fd98a-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="fd98a-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="fd98a-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="fd98a-118">2 </span><span class="sxs-lookup"><span data-stu-id="fd98a-118">2</span></span>|<span data-ttu-id="fd98a-119">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd98a-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="fd98a-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="fd98a-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="fd98a-121">3 </span><span class="sxs-lookup"><span data-stu-id="fd98a-121">3</span></span>|<span data-ttu-id="fd98a-122">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="fd98a-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="fd98a-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="fd98a-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="fd98a-124">4 </span><span class="sxs-lookup"><span data-stu-id="fd98a-124">4</span></span>|<span data-ttu-id="fd98a-125">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="fd98a-125">Audit Windows components, store apps and smart locker.</span></span>|




