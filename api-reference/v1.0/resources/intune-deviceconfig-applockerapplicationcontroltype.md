---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a0f2509aff44de9ebd2c4ae5ea7db63bccfa604f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449138"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="fae07-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fae07-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="fae07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fae07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fae07-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fae07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fae07-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="fae07-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="fae07-107">成员</span><span class="sxs-lookup"><span data-stu-id="fae07-107">Members</span></span>
|<span data-ttu-id="fae07-108">成员</span><span class="sxs-lookup"><span data-stu-id="fae07-108">Member</span></span>|<span data-ttu-id="fae07-109">值</span><span class="sxs-lookup"><span data-stu-id="fae07-109">Value</span></span>|<span data-ttu-id="fae07-110">说明</span><span class="sxs-lookup"><span data-stu-id="fae07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fae07-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fae07-111">notConfigured</span></span>|<span data-ttu-id="fae07-112">0</span><span class="sxs-lookup"><span data-stu-id="fae07-112">0</span></span>|<span data-ttu-id="fae07-113">设备默认值，未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="fae07-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="fae07-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="fae07-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="fae07-115">1</span><span class="sxs-lookup"><span data-stu-id="fae07-115">1</span></span>|<span data-ttu-id="fae07-116">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="fae07-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="fae07-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="fae07-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="fae07-118">双面</span><span class="sxs-lookup"><span data-stu-id="fae07-118">2</span></span>|<span data-ttu-id="fae07-119">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="fae07-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="fae07-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="fae07-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="fae07-121">第三章</span><span class="sxs-lookup"><span data-stu-id="fae07-121">3</span></span>|<span data-ttu-id="fae07-122">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="fae07-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="fae07-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="fae07-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="fae07-124">4 </span><span class="sxs-lookup"><span data-stu-id="fae07-124">4</span></span>|<span data-ttu-id="fae07-125">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="fae07-125">Audit Windows components, store apps and smart locker.</span></span>|







