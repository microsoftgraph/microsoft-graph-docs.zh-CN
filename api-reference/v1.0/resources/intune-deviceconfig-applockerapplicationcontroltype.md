---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 77a47a2654c8e585cadcf48d375d29eedd470991
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755908"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="82647-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="82647-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="82647-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82647-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82647-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82647-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="82647-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="82647-107">成员</span><span class="sxs-lookup"><span data-stu-id="82647-107">Members</span></span>
|<span data-ttu-id="82647-108">成员</span><span class="sxs-lookup"><span data-stu-id="82647-108">Member</span></span>|<span data-ttu-id="82647-109">值</span><span class="sxs-lookup"><span data-stu-id="82647-109">Value</span></span>|<span data-ttu-id="82647-110">Description</span><span class="sxs-lookup"><span data-stu-id="82647-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82647-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="82647-111">notConfigured</span></span>|<span data-ttu-id="82647-112">0</span><span class="sxs-lookup"><span data-stu-id="82647-112">0</span></span>|<span data-ttu-id="82647-113">设备默认值，未选择"应用程序控制"类型。</span><span class="sxs-lookup"><span data-stu-id="82647-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="82647-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="82647-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="82647-115">1</span><span class="sxs-lookup"><span data-stu-id="82647-115">1</span></span>|<span data-ttu-id="82647-116">强制Windows组件和存储应用。</span><span class="sxs-lookup"><span data-stu-id="82647-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="82647-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="82647-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="82647-118">2</span><span class="sxs-lookup"><span data-stu-id="82647-118">2</span></span>|<span data-ttu-id="82647-119">审核Windows组件和存储应用。</span><span class="sxs-lookup"><span data-stu-id="82647-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="82647-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="82647-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="82647-121">3</span><span class="sxs-lookup"><span data-stu-id="82647-121">3</span></span>|<span data-ttu-id="82647-122">强制Windows组件、应用商店应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="82647-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="82647-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="82647-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="82647-124">4 </span><span class="sxs-lookup"><span data-stu-id="82647-124">4</span></span>|<span data-ttu-id="82647-125">审核Windows组件、应用商店应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="82647-125">Audit Windows components, store apps and smart locker.</span></span>|




