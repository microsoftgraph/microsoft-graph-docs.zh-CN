---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937955"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="1e261-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1e261-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="1e261-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e261-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e261-105">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="1e261-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="1e261-106">成员</span><span class="sxs-lookup"><span data-stu-id="1e261-106">Members</span></span>
|<span data-ttu-id="1e261-107">成员</span><span class="sxs-lookup"><span data-stu-id="1e261-107">Member</span></span>|<span data-ttu-id="1e261-108">值</span><span class="sxs-lookup"><span data-stu-id="1e261-108">Value</span></span>|<span data-ttu-id="1e261-109">说明</span><span class="sxs-lookup"><span data-stu-id="1e261-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e261-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1e261-110">notConfigured</span></span>|<span data-ttu-id="1e261-111">0</span><span class="sxs-lookup"><span data-stu-id="1e261-111">0</span></span>|<span data-ttu-id="1e261-112">设备默认值，未选择的应用程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="1e261-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="1e261-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1e261-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="1e261-114">1</span><span class="sxs-lookup"><span data-stu-id="1e261-114">1</span></span>|<span data-ttu-id="1e261-115">强制实施 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1e261-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="1e261-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1e261-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="1e261-117">2</span><span class="sxs-lookup"><span data-stu-id="1e261-117">2</span></span>|<span data-ttu-id="1e261-118">审核 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1e261-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="1e261-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1e261-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1e261-120">3</span><span class="sxs-lookup"><span data-stu-id="1e261-120">3</span></span>|<span data-ttu-id="1e261-121">强制实施 Windows 组件、 存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="1e261-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="1e261-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1e261-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1e261-123">4</span><span class="sxs-lookup"><span data-stu-id="1e261-123">4</span></span>|<span data-ttu-id="1e261-124">审核 Windows 组件，存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="1e261-124">Audit Windows components, store apps and smart locker.</span></span>|



