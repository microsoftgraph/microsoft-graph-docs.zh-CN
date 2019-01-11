---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871979"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="1b422-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b422-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="1b422-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b422-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b422-105">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="1b422-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="1b422-106">成员</span><span class="sxs-lookup"><span data-stu-id="1b422-106">Members</span></span>
|<span data-ttu-id="1b422-107">成员</span><span class="sxs-lookup"><span data-stu-id="1b422-107">Member</span></span>|<span data-ttu-id="1b422-108">值</span><span class="sxs-lookup"><span data-stu-id="1b422-108">Value</span></span>|<span data-ttu-id="1b422-109">Description</span><span class="sxs-lookup"><span data-stu-id="1b422-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b422-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1b422-110">notConfigured</span></span>|<span data-ttu-id="1b422-111">0</span><span class="sxs-lookup"><span data-stu-id="1b422-111">0</span></span>|<span data-ttu-id="1b422-112">设备默认值，未选择的应用程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="1b422-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="1b422-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1b422-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="1b422-114">1</span><span class="sxs-lookup"><span data-stu-id="1b422-114">1</span></span>|<span data-ttu-id="1b422-115">强制实施 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1b422-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="1b422-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1b422-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="1b422-117">2</span><span class="sxs-lookup"><span data-stu-id="1b422-117">2</span></span>|<span data-ttu-id="1b422-118">审核 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1b422-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="1b422-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1b422-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1b422-120">3</span><span class="sxs-lookup"><span data-stu-id="1b422-120">3</span></span>|<span data-ttu-id="1b422-121">强制实施 Windows 组件、 存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="1b422-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="1b422-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1b422-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1b422-123">4</span><span class="sxs-lookup"><span data-stu-id="1b422-123">4</span></span>|<span data-ttu-id="1b422-124">审核 Windows 组件，存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="1b422-124">Audit Windows components, store apps and smart locker.</span></span>|



