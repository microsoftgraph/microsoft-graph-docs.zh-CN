---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: efdb7913d5b813ec528969520e2e7d64da1d3002
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708814"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="02334-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="02334-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="02334-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02334-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02334-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02334-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02334-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02334-107">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="02334-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="02334-108">成员</span><span class="sxs-lookup"><span data-stu-id="02334-108">Members</span></span>
|<span data-ttu-id="02334-109">成员</span><span class="sxs-lookup"><span data-stu-id="02334-109">Member</span></span>|<span data-ttu-id="02334-110">值</span><span class="sxs-lookup"><span data-stu-id="02334-110">Value</span></span>|<span data-ttu-id="02334-111">说明</span><span class="sxs-lookup"><span data-stu-id="02334-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02334-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="02334-112">notConfigured</span></span>|<span data-ttu-id="02334-113">0</span><span class="sxs-lookup"><span data-stu-id="02334-113">0</span></span>|<span data-ttu-id="02334-114">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="02334-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="02334-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="02334-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="02334-116">1</span><span class="sxs-lookup"><span data-stu-id="02334-116">1</span></span>|<span data-ttu-id="02334-117">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="02334-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="02334-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="02334-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="02334-119">双面</span><span class="sxs-lookup"><span data-stu-id="02334-119">2</span></span>|<span data-ttu-id="02334-120">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="02334-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="02334-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="02334-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="02334-122">第三章</span><span class="sxs-lookup"><span data-stu-id="02334-122">3</span></span>|<span data-ttu-id="02334-123">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="02334-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="02334-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="02334-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="02334-125">4 </span><span class="sxs-lookup"><span data-stu-id="02334-125">4</span></span>|<span data-ttu-id="02334-126">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="02334-126">Audit Windows components, store apps and smart locker.</span></span>|





