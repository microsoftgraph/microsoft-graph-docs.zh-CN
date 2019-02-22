---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22d108dd3bad90341031d1e965948a9daa59efa1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141354"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="3411f-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3411f-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="3411f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3411f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3411f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3411f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3411f-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="3411f-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="3411f-107">成员</span><span class="sxs-lookup"><span data-stu-id="3411f-107">Members</span></span>
|<span data-ttu-id="3411f-108">成员</span><span class="sxs-lookup"><span data-stu-id="3411f-108">Member</span></span>|<span data-ttu-id="3411f-109">值</span><span class="sxs-lookup"><span data-stu-id="3411f-109">Value</span></span>|<span data-ttu-id="3411f-110">说明</span><span class="sxs-lookup"><span data-stu-id="3411f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3411f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3411f-111">notConfigured</span></span>|<span data-ttu-id="3411f-112">0</span><span class="sxs-lookup"><span data-stu-id="3411f-112">0</span></span>|<span data-ttu-id="3411f-113">设备默认值, 未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="3411f-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="3411f-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3411f-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="3411f-115">1</span><span class="sxs-lookup"><span data-stu-id="3411f-115">1</span></span>|<span data-ttu-id="3411f-116">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="3411f-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="3411f-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3411f-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="3411f-118">双面</span><span class="sxs-lookup"><span data-stu-id="3411f-118">2</span></span>|<span data-ttu-id="3411f-119">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="3411f-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="3411f-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3411f-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3411f-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3411f-121">3</span></span>|<span data-ttu-id="3411f-122">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="3411f-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="3411f-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3411f-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3411f-124">4</span><span class="sxs-lookup"><span data-stu-id="3411f-124">4</span></span>|<span data-ttu-id="3411f-125">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="3411f-125">Audit Windows components, store apps and smart locker.</span></span>|




