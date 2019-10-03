---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e54aeb4658177531677d875c8b72413f3e4c1ee4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366704"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="6c06c-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6c06c-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="6c06c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c06c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c06c-105">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="6c06c-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="6c06c-106">成员</span><span class="sxs-lookup"><span data-stu-id="6c06c-106">Members</span></span>
|<span data-ttu-id="6c06c-107">成员</span><span class="sxs-lookup"><span data-stu-id="6c06c-107">Member</span></span>|<span data-ttu-id="6c06c-108">值</span><span class="sxs-lookup"><span data-stu-id="6c06c-108">Value</span></span>|<span data-ttu-id="6c06c-109">说明</span><span class="sxs-lookup"><span data-stu-id="6c06c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c06c-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6c06c-110">notConfigured</span></span>|<span data-ttu-id="6c06c-111">0</span><span class="sxs-lookup"><span data-stu-id="6c06c-111">0</span></span>|<span data-ttu-id="6c06c-112">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="6c06c-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="6c06c-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="6c06c-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="6c06c-114">1</span><span class="sxs-lookup"><span data-stu-id="6c06c-114">1</span></span>|<span data-ttu-id="6c06c-115">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="6c06c-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="6c06c-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="6c06c-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="6c06c-117">双面</span><span class="sxs-lookup"><span data-stu-id="6c06c-117">2</span></span>|<span data-ttu-id="6c06c-118">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="6c06c-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="6c06c-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="6c06c-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="6c06c-120">第三章</span><span class="sxs-lookup"><span data-stu-id="6c06c-120">3</span></span>|<span data-ttu-id="6c06c-121">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="6c06c-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="6c06c-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="6c06c-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="6c06c-123">4</span><span class="sxs-lookup"><span data-stu-id="6c06c-123">4</span></span>|<span data-ttu-id="6c06c-124">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="6c06c-124">Audit Windows components, store apps and smart locker.</span></span>|




