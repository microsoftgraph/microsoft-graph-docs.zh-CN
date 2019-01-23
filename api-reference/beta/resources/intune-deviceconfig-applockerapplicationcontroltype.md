---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425720"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0f5d6-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0f5d6-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0f5d6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f5d6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f5d6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f5d6-107">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="0f5d6-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="0f5d6-108">成员</span><span class="sxs-lookup"><span data-stu-id="0f5d6-108">Members</span></span>
|<span data-ttu-id="0f5d6-109">成员</span><span class="sxs-lookup"><span data-stu-id="0f5d6-109">Member</span></span>|<span data-ttu-id="0f5d6-110">值</span><span class="sxs-lookup"><span data-stu-id="0f5d6-110">Value</span></span>|<span data-ttu-id="0f5d6-111">说明</span><span class="sxs-lookup"><span data-stu-id="0f5d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f5d6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0f5d6-112">notConfigured</span></span>|<span data-ttu-id="0f5d6-113">0</span><span class="sxs-lookup"><span data-stu-id="0f5d6-113">0</span></span>|<span data-ttu-id="0f5d6-114">设备默认值，未选择的应用程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0f5d6-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0f5d6-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0f5d6-116">1</span><span class="sxs-lookup"><span data-stu-id="0f5d6-116">1</span></span>|<span data-ttu-id="0f5d6-117">强制实施 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0f5d6-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0f5d6-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0f5d6-119">2</span><span class="sxs-lookup"><span data-stu-id="0f5d6-119">2</span></span>|<span data-ttu-id="0f5d6-120">审核 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0f5d6-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0f5d6-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0f5d6-122">3</span><span class="sxs-lookup"><span data-stu-id="0f5d6-122">3</span></span>|<span data-ttu-id="0f5d6-123">强制实施 Windows 组件、 存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0f5d6-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0f5d6-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0f5d6-125">4</span><span class="sxs-lookup"><span data-stu-id="0f5d6-125">4</span></span>|<span data-ttu-id="0f5d6-126">审核 Windows 组件，存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="0f5d6-126">Audit Windows components, store apps and smart locker.</span></span>|




