---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 07ce6969c79581ed33b3a34d75445f7bf5612598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527075"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="ca07d-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ca07d-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="ca07d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ca07d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca07d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca07d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca07d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca07d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca07d-107">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="ca07d-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="ca07d-108">成员</span><span class="sxs-lookup"><span data-stu-id="ca07d-108">Members</span></span>
|<span data-ttu-id="ca07d-109">成员</span><span class="sxs-lookup"><span data-stu-id="ca07d-109">Member</span></span>|<span data-ttu-id="ca07d-110">值</span><span class="sxs-lookup"><span data-stu-id="ca07d-110">Value</span></span>|<span data-ttu-id="ca07d-111">说明</span><span class="sxs-lookup"><span data-stu-id="ca07d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca07d-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ca07d-112">notConfigured</span></span>|<span data-ttu-id="ca07d-113">0</span><span class="sxs-lookup"><span data-stu-id="ca07d-113">0</span></span>|<span data-ttu-id="ca07d-114">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="ca07d-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="ca07d-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ca07d-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="ca07d-116">1 </span><span class="sxs-lookup"><span data-stu-id="ca07d-116">1</span></span>|<span data-ttu-id="ca07d-117">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="ca07d-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="ca07d-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="ca07d-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="ca07d-119">2 </span><span class="sxs-lookup"><span data-stu-id="ca07d-119">2</span></span>|<span data-ttu-id="ca07d-120">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="ca07d-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="ca07d-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ca07d-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ca07d-122">3 </span><span class="sxs-lookup"><span data-stu-id="ca07d-122">3</span></span>|<span data-ttu-id="ca07d-123">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="ca07d-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="ca07d-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="ca07d-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="ca07d-125">4 </span><span class="sxs-lookup"><span data-stu-id="ca07d-125">4</span></span>|<span data-ttu-id="ca07d-126">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="ca07d-126">Audit Windows components, store apps and smart locker.</span></span>|



