---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
ms.openlocfilehash: 0d6190170d6f6695a3303047f9ccb193afd248f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330203"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="770d9-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="770d9-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="770d9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="770d9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="770d9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="770d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="770d9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="770d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="770d9-107">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="770d9-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="770d9-108">成员</span><span class="sxs-lookup"><span data-stu-id="770d9-108">Members</span></span>
|<span data-ttu-id="770d9-109">成员</span><span class="sxs-lookup"><span data-stu-id="770d9-109">Member</span></span>|<span data-ttu-id="770d9-110">值</span><span class="sxs-lookup"><span data-stu-id="770d9-110">Value</span></span>|<span data-ttu-id="770d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="770d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="770d9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="770d9-112">notConfigured</span></span>|<span data-ttu-id="770d9-113">0</span><span class="sxs-lookup"><span data-stu-id="770d9-113">0</span></span>|<span data-ttu-id="770d9-114">设备默认值，未选择的应用程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="770d9-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="770d9-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="770d9-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="770d9-116">1</span><span class="sxs-lookup"><span data-stu-id="770d9-116">1</span></span>|<span data-ttu-id="770d9-117">强制实施 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="770d9-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="770d9-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="770d9-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="770d9-119">2</span><span class="sxs-lookup"><span data-stu-id="770d9-119">2</span></span>|<span data-ttu-id="770d9-120">审核 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="770d9-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="770d9-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="770d9-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="770d9-122">3</span><span class="sxs-lookup"><span data-stu-id="770d9-122">3</span></span>|<span data-ttu-id="770d9-123">强制实施 Windows 组件、 存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="770d9-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="770d9-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="770d9-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="770d9-125">4</span><span class="sxs-lookup"><span data-stu-id="770d9-125">4</span></span>|<span data-ttu-id="770d9-126">审核 Windows 组件，存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="770d9-126">Audit Windows components, store apps and smart locker.</span></span>|





